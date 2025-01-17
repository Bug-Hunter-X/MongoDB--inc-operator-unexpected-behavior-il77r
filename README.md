# MongoDB $inc Operator Unexpected Behavior

This repository demonstrates a common error related to the MongoDB `$inc` operator. The `$inc` operator is used to increment a numeric field in a document.  However, if used incorrectly, it can lead to unexpected results or data corruption.

## Problem

The primary issue occurs when attempting to increment a field that does not exist. Instead of creating the field and setting it to 1, the $inc operator will do nothing.  Also, incorrect usage with other operators can cause errors.

## Solution

The solution involves using the `$inc` operator correctly within an update operation.  This might require careful consideration of how to handle the case where the field may not exist.