Employee
    String name;
    Int employeeId;

Patient
    String name;
    Int patientId;
    String diagnosis;
    String medication;

Doctor extends Employee
    seePatient (patientId)
    List<Patient> patients;

Cardiologist extends Doctor (Heart doctor)
    String subSpecialty;

Otolaryngologist extends Doctor (Ear nose and throat doctor)

Janitor extends Employee
    sweep ()

Nurse extends Employee
    careForPatient (patientId)
    List<Patient> patients;
