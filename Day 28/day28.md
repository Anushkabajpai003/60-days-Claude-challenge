# 🏥 Hospital Admission Readiness Simulator

## Day 28 of 60 Days Claude Challenge

### Project Overview

The Hospital Admission Readiness Simulator is an interactive healthcare operations training application that places users in the role of a Hospital Admission Coordinator. The simulator focuses on evaluating admission readiness, coordinating stakeholders, managing prior authorization workflows, and reducing admission-related risks.

The application is designed to mirror real-world patient access and utilization review processes while remaining an educational simulation.

---

## Objective

The goal of the simulator is to help users understand how multiple administrative and clinical factors influence hospital admission readiness.

Users must coordinate:

* Prior Authorization (PA)
* Insurance Verification
* Bed Assignment
* Clinical Documentation
* Physician Orders
* Patient Consent
* Care Team Communication

to successfully prepare a patient for admission.

---

## Features

### Admission Setup

Users configure:

* Provider
* Attending Physician
* Diagnosis

  * Acute MI
  * CHF
  * Pneumonia
  * Elective Surgery
  * Hip Fracture
* Admission Type

  * Inpatient
  * Observation
  * Emergency
  * ICU
  * Same-Day Surgery
* PA Status
* Admission Date

---

### Admission Readiness Analysis

The simulator evaluates:

* Prior Authorization Status
* Insurance Verification
* Bed Availability
* Documentation Completeness
* Physician Orders
* Consent Status

and generates an initial readiness score.

### Readiness Score Weighting

| Category               | Weight |
| ---------------------- | ------ |
| PA Status              | 25%    |
| Clinical Documentation | 20%    |
| Physician Orders       | 20%    |
| Insurance              | 15%    |
| Consent                | 10%    |
| Bed Availability       | 10%    |

---

## Prior Authorization Workflow

### Approved

* Continue admission workflow

### Pending

* Follow Up
* Upload Documentation
* Contact Physician

### Denied

* Review Reason
* Contact Insurance
* Submit Appeal

Successful appeals convert the authorization status to Approved.

---

## Clinical Criteria Awareness

For:

* Acute MI
* CHF

The simulator displays:

> InterQual/Milliman thresholds apply — ensure documentation meets medical necessity standards before UR review.

This introduces users to medical necessity review concepts commonly used in healthcare operations.

---

## Timeline Workflow

The admission journey follows:

1. PA Review
2. Insurance Verification
3. Bed Assignment
4. Documentation
5. Consent
6. Patient Arrival
7. Registration
8. Clinical Assessment
9. Admission Complete

---

## Care Coordination Module

The simulator includes key stakeholders:

### Attending Physician

Clinical decision-making and admission approval.

### Case Manager

Care coordination and resource management.

### Nursing

Patient preparation and admission support.

### Utilization Review (UR)

Responsibilities include:

* Concurrent Review
* Denial Risk Identification
* InterQual Review
* Milliman Criteria Assessment

### Discharge Planner

Early discharge planning and transition preparation.

---

## Risk Tracking

The simulator continuously evaluates:

* Documentation Risk
* Insurance Risk
* Bed Risk
* Clinical Risk

Clinical risk receives additional weighting for:

* Acute MI
* CHF
* ICU Admissions

---

## Governance Snapshot

When readiness reaches 75% or higher, benchmark insights appear:

* PA Turnaround: 3–5 Days
* Inpatient Denial Rate: ~8–10%
* PA Rework Cost: ~$11 per Transaction

*Benchmarks are educational estimates and not intended for operational decision-making.*

---

## Final Decision Logic

### ✅ Admit (90%+ Readiness)

Requirements met:

* Authorization completed
* Documentation finalized
* Orders verified
* Consent completed
* Risks mitigated

A complete admission summary is generated.

### ⚠ Not Ready (<90% Readiness)

The simulator identifies:

* Missing Requirements
* Outstanding Tasks
* Remaining Risks
* Recommended Next Actions

---


## Key Learnings

* Hospital admissions require coordination across multiple departments.
* Prior authorization significantly impacts admission readiness.
* Documentation quality influences medical necessity reviews.
* Utilization Review teams help reduce denial risk.
* Administrative readiness and clinical readiness must work together.
* Early risk identification improves admission efficiency.

---

## Technologies Used

* HTML
* Tailwind CSS
* Vanilla JavaScript

---

## Challenge Progress

✅ Day 28 Complete

Building practical healthcare operations simulations to better understand patient access, utilization review, and admission workflows.

#60DayClaudeChallenge
