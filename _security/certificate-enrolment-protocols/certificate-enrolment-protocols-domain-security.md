---
api_specs:
- filename: certificate-enrolment-protocols-openapi.yml
  format: yaml
  label: ACME - Automatic Certificate Management Environment (RFC 8555)
  slug: acme-rfc-8555
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certificate-enrolment-protocols/refs/heads/main/openapi/certificate-enrolment-protocols-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wikipedia.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ietf.org
  spf: true
hosts:
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: en.wikipedia.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 20:01:07 2026 GMT
  host: datatracker.ietf.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 05:24:45 2026 GMT
  host: cert-manager.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Certificate Enrolment Protocols Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certificate Enrolment Protocols, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Certificate Enrolment Protocols
provider_slug: certificate-enrolment-protocols
slug: certificate-enrolment-protocols-domain-security
source_filename: certificate-enrolment-protocols-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.wikipedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: datatracker.ietf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:01:07 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: cert-manager.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:24:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wikipedia.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ietf.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certificate-enrolment-protocols/refs/heads/main/security/certificate-enrolment-protocols-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- ACME
- Automation
- CMP
- Certificates
- Cryptography
- EST
- IETF
- Let's Encrypt
- PKI
- RFC
- Renewal
- SCEP
- Security
- Standards
---
