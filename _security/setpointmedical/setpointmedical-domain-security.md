---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "www.digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: setpointmedical.com
  spf: true
hosts:
- cert_expires: Sep 15 02:03:30 2026 GMT
  host: setpointmedical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Setpointmedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Setpointmedical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Setpointmedical
provider_slug: setpointmedical
slug: setpointmedical-domain-security
source_filename: setpointmedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: setpointmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:03:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: setpointmedical.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"www.digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/setpointmedical/refs/heads/main/security/setpointmedical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Medical Device
- Bioelectronic Medicine
- Neuromodulation
- Rheumatoid Arthritis
- Healthcare
- Implantable Device
---
