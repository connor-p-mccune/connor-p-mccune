# Hi, I'm Connor 👋

**Computer Science student at Florida Polytechnic University with a concentration in cybersecurity. I'm mainly focused on GRC and cloud security.** I build Python tools that check AWS environments against NIST SP 800-171 and turn the results into audit-ready evidence.

- 🎓 B.S. Computer Science, Cybersecurity concentration · Class of 2028 · 3.74 GPA
- 🛡️ Focus: NIST SP 800-171/171A, NIST SP 800-53, CMMC, DoD SPRS scoring, cloud security posture
- 📜 CompTIA Security+ exam scheduled for January 2027
- 🇺🇸 U.S. citizen, eligible for a security clearance
- 🔎 Looking for Summer 2027 internships in GRC, cybersecurity compliance, or cloud security

## Featured project

### [NIST SP 800-171 AWS Compliance Scanner](https://github.com/connor-p-mccune/nist171-collector)

A Python CLI that audits an AWS account against NIST SP 800-171 Rev 2, separates failed controls from requirements that need manual review, and calculates a DoD SPRS score.

- **Coverage:** 15 of 110 requirements automated across the AC, AU, and IA families; all 110 modeled in YAML with DoD point values, 800-53 Rev 4 mappings, and 800-171A objectives
- **Scoring:** SPRS per DoD Assessment Methodology v1.2.1, including 3.5.3 MFA partial credit and N/A exceptions; unassessed requirements are reported separately so the score never overstates compliance
- **Collection:** 5 read-only boto3 collectors (IAM, CloudTrail, EC2, S3, KMS) running under a least-privilege SecurityAudit identity
- **Evidence:** every API response saved as SHA-256-hashed, timestamped evidence for a tamper-evident audit trail
- **Checks:** 19 automated checks with a 5-state verdict model and remediation guidance for every failure
- **Testing:** validated against a non-compliant, Terraform-provisioned AWS environment; all 19 checks unit-tested with pytest and moto

`Python` `boto3` `AWS` `Terraform` `pytest` `moto` `YAML`

## More projects

- **[vulnpipe](https://github.com/connor-p-mccune/vulnpipe)** — Network + web vulnerability scanning pipeline that orchestrates Nmap and OWASP ZAP, enriches findings with CVSS/CVE/EPSS, and outputs prioritized HTML/JSON/SARIF reports with a CI gate
- **[netsentry](https://github.com/connor-p-mccune/netsentry)** — ML network intrusion detection that pairs a supervised classifier for known attacks with an anomaly detector for novel ones, served behind a real-time API with explainable predictions

## Toolbox

| Area | Tools & frameworks |
|---|---|
| GRC | NIST SP 800-171/171A · NIST SP 800-53 · CMMC · DoD Assessment Methodology (SPRS) · POA&M |
| Cloud security | AWS (IAM, CloudTrail, Security Groups, EC2, S3, KMS) · Terraform · least privilege · audit logging |
| Security tools | Nmap · Wireshark · Gitleaks |
| Languages | Python · Bash · PowerShell · SQL · C++ · C · Java · HCL · YAML |
| Platforms | Linux · Docker · Git/GitHub · Active Directory · VS Code |

## Connect

[LinkedIn](https://www.linkedin.com/in/connor-p-mccune) · [Email](mailto:connor.p.mccune@gmail.com)
