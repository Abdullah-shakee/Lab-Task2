# TASK A — DEFECT HUNT  
## Online Course Registration System

---

# 1. Inconsistencies (5+ Required)

## 1) R2 vs R3 Conflict
- **R2:** Registration is not allowed after the deadline.  
- **R3:** Late registration is allowed for 3 days after the deadline.  

**Issue:**  
There is a conflict about whether registration is allowed after the deadline.  
These two requirements directly contradict each other.

---

## 2) R4 vs R5 vs R16 Conflict
- **R4:** The system shall show available seats.  
- **R5:** Students can register even if seats are full.  
- **R16:** The system shall support waitlisting when seats are full.  

**Issue:**  
If seats are full, should the system:
- Register the student directly?  
- Place the student on a waitlist?  

The behavior is unclear and conflicting.

---

## 3) R9 vs R10 Conflict
- **R9:** The system shall prevent schedule conflicts.  
- **R10:** Students may register for two courses at the same time if one is online.  

**Issue:**  
There is a direct contradiction unless an exception rule is clearly defined.  
The general rule conflicts with the exception.

---

## 4) R11 vs R12 Conflict
- **R11:** Limit students to 18 credit hours per semester.  
- **R12:** Allow up to 24 credit hours with advisor approval.  

**Issue:**  
The limit is unclear — is 18 strict or conditional?  
The base rule and exception are not clearly connected.

---

## 5) R13 vs R14 vs R15 Conflict
- **R13:** Students may drop courses until Week 6.  
- **R14:** The system shall charge a fee after Week 2.  
- **R15:** The system shall not allow course drops after the deadline.  

**Issue:**  
The deadline is not defined.  
This creates confusion about the actual drop policy.

---

# 2. Incompleteness (5+ Required)

## 1) R1 is Incomplete
It does not mention:
- Registration period  
- Credit hour limits  
- Conditions for registration  

---

## 2) R6 is Incomplete
“The system shall send confirmation.”

Missing:
- Email or SMS?  
- When it will be sent?  
- What information it includes?  

---

## 3) R8 is Incomplete
It states prerequisites may be ignored with instructor approval, but:
- How is approval given?  
- Is it recorded in the system?  

---

## 4) R16 is Incomplete
Waitlist behavior is unclear:
- Is there a maximum waitlist size?  
- Will students be notified?  

---

## 5) R19 is Incomplete
Priority enrollment is mentioned, but:
- How is priority given?  
- How long does priority last?  

---

# 3. Ambiguities (3+ Required)

## 1) R2 – “Deadline” is unclear
It does not specify which deadline:
- Registration deadline  
- Semester deadline  

---

## 2) R5 – “Allow registration even if seats are full”
It is unclear whether this means:
- Over-enrollment  
- Automatic waitlisting  

---

## 3) R20 – “Register quickly”
The word “quickly” has no measurable meaning.

---

# 4. Unverifiable Requirements (2+ Required)

## 1) R20 – Unverifiable
There is no measurable time defined for “quickly,” so it cannot be tested.

---

## 2) R6 – Unverifiable
Since the confirmation method and timing are not defined, testers cannot verify it.

---

# Summary

Total Defects Identified:

- 5 Inconsistencies  
- 5 Incompleteness Issues  
- 3 Ambiguities  
- 2 Unverifiable Requirements  

Minimum requirements satisfied.