# Privacy and clinical authority

| Path | Who can read the contents |
| --- | --- |
| Public offline case | The device holds the fictional records. Service events in this case are simulated. |
| Connected care messages | Authorised endpoints read messages after decryption. The relay stores ciphertext and routing or delivery information. |
| Optional Azure AI | The gateway and model can read only the selected text submitted for processing. Patients review the excerpt before sharing. |
| Consented deadline | The scheduler can use a deadline, status and opaque route to queue an already encrypted envelope. |

The connected test uses scoped, synthetic enrolment. An invitation expires and can be used once. The patient reviews the identity and scope before acceptance. Connection keys are bound to the authorised endpoints. The transport records queued, accepted and delivered separately from clinician acknowledgement.

Request limits, source versions and response checks keep the optional AI flow bounded. Identifier minimisation is best effort. A correction can invalidate earlier derived text and a verified stop cancels affected future tasks. When connectivity is unavailable, the app keeps accepted instructions visible and can queue eligible messages. A queue or receipt offers no guarantee of a clinical response.

The public app is a competition build with fictional data. Live clinical use requires a responsible facility, validated data interfaces, a staffed response process, independent review, and agreed recovery and retention policies.

[System architecture](architecture.md) · [Verification and limitations](verification.md) · [Documentation home](README.md)
