---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:support@high-t.co.il"
  - 0 issue ";"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bio-beat.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bio-beat.cloud
  spf: true
hosts:
- cert_expires: Sep 23 05:05:46 2026 GMT
  host: www.bio-beat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: remote-monitoring.us.bio-beat.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.us.bio-beat.cloud
  https: false
kind: domain-security
layout: security
method: probed
name: Biobeat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biobeat, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biobeat
provider_slug: biobeat
slug: biobeat-domain-security
source_filename: biobeat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bio-beat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:05:46 2026 GMT\n  hsts: false\n- host: remote-monitoring.us.bio-beat.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\n- host: api.us.bio-beat.cloud\n  https: false\ndomains:\n- domain: bio-beat.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:support@high-t.co.il\"\n  - 0 issue \";\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bio-beat.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biobeat/refs/heads/main/security/biobeat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Remote Patient Monitoring
- RPM
- Wearables
- Vital Signs
- Cuffless Blood Pressure
- Digital Health
- Medical Devices
- PPG
- Partner Gated
---
