# Functional Specification Document: Visa Base II Offline Outgoing Interface

## 1. Introduction

This Functional Specification Document (FSD) outlines the requirements and specifications for the Visa Base II Offline Outgoing Interface within the financial institution CPLS's interchange system.

## 2. System Overview

The Visa Base II Offline Outgoing Interface is part of the larger interchange system for CPLS. It is designed to handle outgoing transactions and communications with the Visa network using the Base II protocol.

## 3. Functional Requirements

### 3.1 Interface Identification
- ID: 222
- Class: Visa Base II Offline Outgoing Interface
- Name: VISA 1

[Source: frame_000338.md]

### 3.2 File Handling
- File name template: <not defined>
- File name generator: <not defined>
- File name generation function: <not defined>
- File encoding: ASCII
- File packing: <none>
- Services' client profile for file processing: <take from executing party instance>

[Source: frame_000338.md]

### 3.3 Visa Processing
- Visa processing BIN: 455555
- Start sequence number: 0
- Minimum sequence number: 0
- Maximum sequence number: 0
- Maximum number of records: 999
- File type: Center Transaction File

[Source: frame_000338.md]

### 3.4 Settlement Configuration
- National settlement: National Net settlement service (valid only for countries with defined service)
- International settlement: BASE II selects the appropriate settlement service based on routing and country-defined default
- Settlement type: No deferment

[Source: frame_000338.md]

### 3.5 Export Configuration
- Post-export OS command: <not defined>
- Maximum records per file: <unlimited>
- Message correction function: <not defined>

[Source: frame_000339.md]

### 3.6 Batch Export Types
- Batch type for incremental export: <not defined>
- Batch type for response export: <not defined>
- Batch type for chargeback export: <not defined>
- Batch type for fee export: <not defined>
- Batch type for funds transfer export: <not defined>
- Batch type for retrieval request export: <not defined>

[Source: frame_000339.md]

### 3.7 Export Progress Tracking
- Incremental export in progress: <not defined>
- Response export in progress: <not defined>
- Chargeback export in progress: <not defined>
- Fee export in progress: <not defined>
- Funds transfer export in progress: <not defined>
- Retrieval request export in progress: <not defined>

[Source: frame_000339.md]

## 4. Non-Functional Requirements

### 4.1 Performance
- The system must handle a maximum of 999 records per file.

[Source: frame_000338.md]

### 4.2 Security
- File encoding is set to ASCII to ensure proper character representation.

[Source: frame_000338.md]

### 4.3 Compatibility
- The interface must be compatible with Visa's Base II protocol and Center Transaction File type.

[Source: frame_000338.md]

## 5. System Architecture

The Visa Base II Offline Outgoing Interface is part of the larger interchange system within the CPLS financial institution. It interacts with other components such as:

- Routes
- Network Routes
- Range Tables
- Network Structures
- Core Banking Authorization Hosts
- Interchange Contracts
- Settlement Contracts
- Settlement Contract Types
- Interchange Fee Tariff Plans
- Service Bus Pipelines

[Source: frame_000324.md]

## 6. Data Management

The interface handles outgoing transaction data in the form of files. Key data management aspects include:

- File naming and generation (currently not defined)
- ASCII encoding for file contents
- No specific file packing method
- Handling of various transaction types (incremental, response, chargeback, fee, funds transfer, retrieval request)

[Sources: frame_000338.md, frame_000339.md]

## 7. Interface Specifications

The Visa Base II Offline Outgoing Interface (ID: 222) is designed to handle outgoing communications with the Visa network. It processes Center Transaction Files and manages various types of exports including incremental, response, chargeback, fee, funds transfer, and retrieval request exports.

[Sources: frame_000338.md, frame_000339.md]

## 8. Testing Requirements

While specific testing requirements are not provided in the research report, the following areas should be considered for testing:

- File generation and naming
- Correct encoding (ASCII) of file contents
- Proper handling of different export types
- Adherence to maximum record limits (999 per file)
- Correct application of settlement configurations

## 9. Deployment and Maintenance

The interface is part of the CPLS financial institution's interchange system. Specific deployment and maintenance procedures are not provided in the research report but should be aligned with the overall system's practices.

## 10. Conclusion

This Functional Specification Document outlines the key requirements and specifications for the Visa Base II Offline Outgoing Interface (VISA 1) within the CPLS financial institution's interchange system. It provides a foundation for development, testing, and implementation of the interface to ensure proper communication with the Visa network using the Base II protocol.