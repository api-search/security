---
api_specs:
- filename: virus
  format: yaml
  label: Cloudmersive Virus Scan API
  slug: cloudmersive-virus-scan-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/virus
- filename: security
  format: yaml
  label: Cloudmersive Security Threat Detection API
  slug: cloudmersive-security-threat-detection-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/security
- filename: spam
  format: yaml
  label: Cloudmersive Spam Detection API
  slug: cloudmersive-spam-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/spam
- filename: phishing
  format: yaml
  label: Cloudmersive Phishing Detection API
  slug: cloudmersive-phishing-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/phishing
- filename: cdr
  format: yaml
  label: Cloudmersive Content Disarm and Reconstruction (CDR) API
  slug: cloudmersive-cdr-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/cdr
- filename: fraud
  format: yaml
  label: Cloudmersive Fraud Detection API
  slug: cloudmersive-fraud-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/fraud
- filename: dlp
  format: yaml
  label: Cloudmersive Data Loss Prevention (DLP) API
  slug: cloudmersive-dlp-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/dlp
- filename: convert
  format: yaml
  label: Cloudmersive Document Convert API
  slug: cloudmersive-convert-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/convert
- filename: barcode
  format: yaml
  label: Cloudmersive Barcode API
  slug: cloudmersive-barcode-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/barcode
- filename: image
  format: yaml
  label: Cloudmersive Image Recognition and Processing API
  slug: cloudmersive-image-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/image
- filename: nlp
  format: yaml
  label: Cloudmersive Natural Language Processing API
  slug: cloudmersive-nlp-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/nlp
- filename: ocr
  format: yaml
  label: Cloudmersive OCR API
  slug: cloudmersive-ocr-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/ocr
- filename: speech
  format: yaml
  label: Cloudmersive Speech API
  slug: cloudmersive-speech-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/speech
- filename: validate
  format: yaml
  label: Cloudmersive Validate API
  slug: cloudmersive-validate-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/validate
- filename: video
  format: yaml
  label: Cloudmersive Video API
  slug: cloudmersive-video-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/video
- filename: currency
  format: yaml
  label: Cloudmersive Currency API
  slug: cloudmersive-currency-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/currency
- filename: config
  format: yaml
  label: Cloudmersive Configuration API
  slug: cloudmersive-config-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/config
- filename: dataintegration
  format: yaml
  label: Cloudmersive Data Integration API
  slug: cloudmersive-data-integration-api
  spec_type: OpenAPI
  url: https://api-console.cloudmersive.com/swagger/api/dataintegration
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cloudmersive.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: cloudmersive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudmersive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudmersive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cloudmersive
provider_slug: cloudmersive
slug: cloudmersive-domain-security
source_filename: cloudmersive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudmersive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cloudmersive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudmersive/refs/heads/main/security/cloudmersive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Barcodes
- Conversions
- Documents
- Image Recognition
- Natural Language
- OCR
- Processing
- Validation
- Virus Scanning
---
