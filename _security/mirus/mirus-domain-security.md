---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mirusmed.com
  spf: true
hosts:
- cert_expires: Nov 19 23:01:33 2026 GMT
  host: www.mirusmed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: rpm.mirusmed.com
  hsts: null
  https: true
  note: GALILEO / "Mirus Analytics" clinician application (CloudFront + S3 SPA). Its /api/* routes, including /api/v1/fhir, answer 401 to anonymous requests.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mirus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MiRus, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MiRus
provider_slug: mirus
slug: mirus-domain-security
source_filename: mirus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mirusmed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:01:33 2026 GMT\n  hsts: null\n- host: rpm.mirusmed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n  note: >-\n    GALILEO / \"Mirus Analytics\" clinician application (CloudFront + S3 SPA). Its /api/* routes,\n    including /api/v1/fhir, answer 401 to anonymous requests.\ndomains:\n- domain: mirusmed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnotes:\n- www.mirusmed.com completes a TLS handshake but silently drops anonymous HTTP requests for\n  dynamic (WordPress) paths — /, /contact/, /wp-json/ all time out with no bytes returned —\n  while static /wp-content/ assets on the same host return 200. Recorded as observed; not\n  treated as a dead host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirus/refs/heads/main/security/mirus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Life Sciences
- Spine
- Orthopaedics
- Structural Heart
- Remote Patient Monitoring
- Medical Implants
- Surgical Planning
---
