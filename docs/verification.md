# Verification and limitations

**Public build:** Android `0.5.0-synthetic`, version code 2, minimum API 31. A clean install passed on Android 16. The competition APK uses Android APK Signature Scheme v2 with debug signing. [APK and checksum](https://github.com/bakkey/inayati-review/releases/tag/v0.5.0-synthetic)

| Area | Observed result |
| --- | --- |
| Native app | 73 unit tests, 9 Android tests, two encrypted-vault restart probes and 44 bilingual screen captures. Lint reported zero errors and one warning. |
| Reviewer access | A hosted runner verified anonymous downloads of the APK, quick start and original working-app recording. [Verification run](https://github.com/bakkey/inayati-review/actions/runs/44694788493) |
| Timing and offline access | The timeline showed 21:20 and the already-due 09:50 check-in. The saved Care screen reopened in airplane mode at 130% text size. |
| Connected workflow | Two enrolled Android emulators exercised queue and retry, an encrypted reply, a corrected result, a stopped order, attendance and clinician closure. The inspected relay storage and logs lacked the test’s synthetic clinical plaintext markers. |
| Device services | Reminder delivery, cancellation on stop, denied permissions and restart/timezone recovery were exercised. English and Arabic typed review and cancellation passed. |
| Optional AI | Controlled Azure tests used synthetic inputs. Public offline explanations are simulated. |

The design assumes clear, versioned clinician instructions, patient confirmation of reports and someone accountable for live follow-up. A public connected relay and self-enrolment remain pending. Spoken transcription on physical devices remains unverified. There is no live Abu Dhabi clinical integration. Independent security review, production recovery and clinical validation are future work.

[Download the full guide and archived test records](https://github.com/bakkey/inayati-review/releases/download/v0.5.0-synthetic/Inayati-Full-Technical-Documentation.pdf) · [Future improvements](roadmap.md) · [Documentation home](README.md)
