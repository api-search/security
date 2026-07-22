---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: helloheart.com
  spf: true
hosts:
- cert_expires: Aug 20 06:26:28 2026 GMT
  host: www.helloheart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hello Heart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hello Heart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hello Heart
provider_slug: hello-heart
slug: hello-heart-domain-security
source_filename: hello-heart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helloheart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:26:28 2026 GMT\n  hsts: false\ndomains:\n- domain: helloheart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hello-heart/refs/heads/main/security/hello-heart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Cardiovascular
- Blood Pressure
- Hypertension
- Remote Patient Monitoring
- Health AI
- Employer Benefits
---
