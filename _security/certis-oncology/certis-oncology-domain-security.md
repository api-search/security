---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: certisoncology.com
  spf: true
hosts:
- cert_expires: Dec 24 00:07:36 2026 GMT
  host: www.certisoncology.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Certis Oncology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certis Oncology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Certis Oncology
provider_slug: certis-oncology
slug: certis-oncology-domain-security
source_filename: certis-oncology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.certisoncology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 00:07:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: certisoncology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certis-oncology/refs/heads/main/security/certis-oncology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Oncology
- AI
- Precision-Medicine
- Preclinical
---
