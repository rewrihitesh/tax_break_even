# AI Tax Filing Agent - Project Scope

## Mission

Build an AI-assisted Indian Income Tax Filing Agent that helps taxpayers complete their tax returns with minimal manual effort.

The system should:

1. Analyze government-provided and taxpayer-provided documents.
2. Identify the correct ITR form.
3. Detect missing information.
4. Suggest deductions and optimizations.
5. Compare old vs new tax regimes.
6. Generate a complete and valid filing package.
7. Keep a human in control of all final decisions.

The goal is not to replace the taxpayer.

The goal is to dramatically reduce the effort required to complete an accurate tax return.

---

## Product Vision

The user should be able to:

```text
Upload documents
-> Answer a small number of questions
-> Receive recommendations
-> Review generated return
-> Approve filing package
```

The agent should perform most of the work.

The human should provide supervision and final approval.

---

## Out of Scope

The project will NOT initially support:

- Direct filing to the Income Tax Portal
- Browser automation
- Login automation
- CA workflow management
- GST filing
- Corporate taxation
- Partnership firm taxation
- Trust taxation
- International tax planning
- Tax litigation
- Notice response automation
- Appeals and assessments
- Audit support

These may be future enhancements.

---

## Target Users

Phase 1:

- Resident Individuals
- Salaried Employees
- Basic Investors

Phase 2:

- Individuals with Capital Gains
- Multiple Income Sources
- Rental Income

Phase 3:

- Freelancers
- Consultants
- Professionals
- Business Owners

---

## Supported Forms

### Phase 1

- ITR-1

### Phase 2

- ITR-2

### Phase 3

- ITR-3

No other forms are currently planned.

---

## Core Principle

Tax calculations and validations must be deterministic.

AI must not be the source of truth.

AI is responsible for:

- Document understanding
- Information extraction
- User interviews
- Missing data detection
- Recommendations
- Explanations

Rule engines are responsible for:

- Eligibility determination
- Tax calculations
- Validation
- Compliance checks

---

## Primary Inputs

The system should be designed around the following inputs:

### Government Sources

- Prefilled Return Data
- AIS
- Form 26AS

### User Sources

- Form 16
- Previous Return
- Broker Statements
- Capital Gain Statements
- Home Loan Certificates
- Investment Proofs
- Bank Statements

---

## Phase 1 Success Criteria

A user uploads:

- Prefilled JSON
- Form 16

The system should:

1. Determine the correct ITR form.
2. Build a taxpayer profile.
3. Ask only necessary questions.
4. Detect missing deductions.
5. Compare tax regimes.
6. Generate a valid return package.
7. Produce a review report.

---

## Human Review Requirement

Every filing package must contain:

### Agent Findings

- Missing Information
- Assumptions
- Recommendations

### Validation Results

- Errors
- Warnings
- Compliance Checks

### Filing Summary

- Selected ITR
- Tax Regime
- Tax Liability
- Refund or Tax Due

Human approval is mandatory before filing.

---

## Research Objectives

The agent must continuously improve understanding of:

- ITR eligibility rules
- Tax calculation rules
- AIS interpretation
- Form 26AS interpretation
- Prefilled JSON structure
- Common filing mistakes
- Deduction opportunities
- Validation requirements

All research must be traceable to official government documentation whenever possible.

---

## Non-Functional Requirements

The system must:

- Be explainable
- Be auditable
- Be versioned by Assessment Year
- Maintain data lineage
- Support manual overrides
- Preserve all user decisions
- Generate reproducible outputs

---

## Definition of Success

The project succeeds when a taxpayer can:

```text
Upload tax documents
-> Answer a small set of questions
-> Receive accurate recommendations
-> Review the result
-> Generate a filing-ready package
```

without needing detailed knowledge of the Income Tax Act or ITR forms.