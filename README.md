## API Testing Project - Urban Grocers

# Project Overview
This project focuses on testing the API functionalities for "Working with Kits" and "Working with Deliveries" in the Urban Grocers system. The goal is to ensure the proper working of these features through API testing, identify any defects, and report them appropriately.

# Testing Strategy
Requirement Analysis: Studied API documentation and decomposed requirements.
Test Case Design: Created test cases based on equivalence partitioning and boundary value analysis.
Test Execution: Ran test cases using Postman.
Bug Tracking: Logged issues in Jira.
Test Reporting: Documented test results to summarize findings and coverage.

# Test Coverage Summary

Requirement 1: Working with Kits

Ensured users can add existing products to a kit via POST /api/v1/kits/:id/products.
Validated product limit constraints (max 30 items per kit).
Checked error handling:
400 Bad Request for invalid product IDs.
404 Not Found for non-existent kit IDs.
400 Bad Request for incorrect request structures.

Requirement 2: Working with Deliveries
Verified the "Fast Delivery" service works when Shipping Price Calculation Requirements are met.
Tested endpoint POST /fast-delivery/v3.1.1/calculate-delivery.xml with various scenarios:
deliveryTime: Verified against the Operating Hours.
productsWeight: Ensured different weights affect pricing correctly.
productsCount: Checked order eligibility based on quantity.

Bug reports are available on links at the comment section to the test cases
