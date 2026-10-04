# Technical Whitepaper — AIDBOX

**Model:** PAX L5 Narrow L2 General 27B
**Company:** Anticloud FZ LLE
**Upstream:** https://github.com/HealthSamurai/aidbox
**Category:** HOSPITAL_AI

## Abstract

This whitepaper describes the Anticloud integration of `AIDBOX` (FHIR API server for hospitals)
with PAX L5 Narrow L2 General 27B, the offline-first AI model developed by Anticloud FZ LLE.
The integration produces a zero-cloud, single-binary deployment that exceeds upstream
capabilities while eliminating all third-party API dependencies.

## Technical Improvements

1. PAX L5 Narrow L2 General 27B local clinical NLP — air-gapped hospital deployment
2. AIOSS HIPAA-aligned audit chain for all AI inference on patient data
3. AES-256 encryption for all PHI processed by AI pipeline
4. Single-binary deployment on clinical GPU workstations
5. Zero-cloud: all model inference, logging, and storage on hospital network
6. GPU/CPU equalizer: radiology AI on GPU, NLP triage on CPU
7. Explainability module: local attention visualization, no cloud XAI API
8. HL7 FHIR R4 integration replacing proprietary HL7 v2 middleware

## Architecture

See TECHNICAL/01_Architecture.md for the full architectural description.

## Benchmarks

See OFFICIAL_BENCHMARKS/04_PAX_Results.md for performance targets and measured results.