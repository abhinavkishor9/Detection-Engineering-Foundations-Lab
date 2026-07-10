# Troubleshooting Notes

## Challenge 1

Understanding how detection engineering differs from traditional log monitoring.

### Resolution

Focused on attacker behaviors, detection logic, and event correlation instead of individual security events.

---

## Challenge 2

Developing effective Sigma rules.

### Resolution

Used Sigma rule structure to define meaningful detection logic while minimizing false positives through contextual filtering.

---

## Challenge 3

Investigating PowerShell activity.

### Resolution

Correlated PowerShell execution with process creation, encoded commands, and related endpoint activity to improve confidence.

---

## Challenge 4

Detecting Certutil abuse.

### Resolution

Identified suspicious command-line switches and correlated Certutil usage with network activity and file downloads.

---

## Challenge 5

Analyzing RDP authentication events.

### Resolution

Reviewed failed and successful logons together to identify potential brute-force attacks while considering legitimate administrative access.

---

## Challenge 6

Reducing False Positives

### Resolution

Validated alerts using user context, administrative activity, parent-child process relationships, and supporting telemetry before classifying them as malicious.

---

## Challenge 7

Mapping detections to MITRE ATT&CK.

### Resolution

Mapped each detection to the appropriate ATT&CK tactic and technique to standardize investigations and identify detection gaps.

---

## Lessons Learned

- Effective detections require contextual analysis rather than isolated events.
- Correlating multiple telemetry sources significantly improves detection fidelity.
- Detection tuning is essential for reducing false positives.
- MITRE ATT&CK provides a consistent framework for detection engineering and incident investigations.
- Continuous coverage assessment helps prioritize future detection development.
