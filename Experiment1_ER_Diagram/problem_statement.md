# Experiment 1: Entity-Relationship (ER) Diagram

## 🎯 Objective:
To understand and apply the concepts of ER modeling by creating an ER diagram for a real-world application.

## 📚 Purpose:
The purpose of this workshop is to gain hands-on experience in designing ER diagrams that visually represent the structure of a database including entities, relationships, attributes, and constraints.

---

## 🧪 Choose One Scenario:

### 🔹 Scenario 1: University Database
Design a database to manage students, instructors, programs, courses, and student enrollments. Include prerequisites for courses.

**User Requirements:**
- Academic programs grouped under departments.
- Students have admission number, name, DOB, contact info.
- Instructors with staff number, contact info, etc.
- Courses have number, name, credits.
- Track course enrollments by students and enrollment date.
- Add support for prerequisites (some courses require others).

---

### 🔹 Scenario 2: Hospital Database
Design a database for patient management, appointments, medical records, and billing.

**User Requirements:**
- Patient details including contact and insurance.
- Doctors and their departments, contact info, specialization.
- Appointments with reason, time, patient-doctor link.
- Medical records with treatments, diagnosis, test results.
- Billing and payment details for each appointment.

---

## 📝 Tasks:
1. Identify entities, relationships, and attributes.
2. Draw the ER diagram using any tool (draw.io, dbdiagram.io, hand-drawn and scanned).
3. Include:
   - Cardinality & participation constraints
   - Prerequisites for University OR Billing for Hospital
4. Explain:
   - Why you chose the entities and relationships.
   - How you modeled prerequisites or billing.

# ER Diagram Submission - Student Name

## Scenario Chosen:
University / Hospital (choose one)

## ER Diagram:
![image](https://github.com/user-attachments/assets/cd4c167b-c1e0-4f04-abfc-f69536923028)


## Entities and Attributes:
Doctors

Attributes: Name, Address, Specialization, Qualification

Patients

Attributes: Disease Type, Details

Pharmacy

Attributes: Medicines

Tests

Attributes: Type, Description

Log

Attributes: Report, Date

Prescriptions, Treatment, Management, Records

No attributes shown in the diagram
## Relationships and Constraints:

# Relationships:
Doctors treat Patients (1-to-many)

Doctors give Prescriptions (1-to-many)

Patients receive Treatment (1-to-many)

Patients have Logs (1-to-many)

Logs include Tests (1-to-many)

Pharmacy supplies Medicines (1-to-many)

Pharmacy links with Doctors and Patients (many-to-many)

Management maintains Records (1-to-many)

Doctors are managed by Management (many-to-one)

# Constraints:
A doctor can treat many patients, but each patient has one doctor.

Each patient can have multiple logs and treatments.

Logs must have at least one test.

Pharmacy can serve both doctors and patients.

Each entity should have a unique ID (implied).
## Extension (Prerequisite / Billing):

# Prerequisite

Attributes: RequirementType, Description

Linked to: Tests, Treatment

Purpose: Defines necessary steps before tests or treatment (e.g., fasting, consent)

# Billing

Attributes: BillID, Amount, PaymentStatus, Date

Linked to: Patients, Treatment, Pharmacy

Purpose: Tracks costs for treatments, medicines, and services



## Design Choices:
The design includes core entities such as Doctors, Patients, Pharmacy, Treatment, Tests, and Prescriptions to represent essential healthcare processes. Logs and Records are used to separately track patient interactions and hospital documentation. The addition of Prerequisite ensures that necessary conditions (e.g., fasting, consent) are met before tests or treatments. Billing is included to manage payments related to treatments and medicines. Relationships are defined to show how doctors treat patients, prescribe medication, and are managed by the hospital. Patients undergo treatments, tests, and have activity logs. The pharmacy interacts with both doctors and patients. Billing is linked to services received. Key assumptions include one doctor treating a patient at a time, all procedures having possible prerequisites, and each service generating a billing record.

## RESULT
Thus, the ER diagram for hospital management has been executed successfully.
