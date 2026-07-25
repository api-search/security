---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: storsimple.com
  spf: true
hosts:
- host: www.storsimple.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.storsim'
kind: domain-security
layout: security
method: probed
name: Storsimple Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StorSimple, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StorSimple
provider_slug: storsimple
slug: storsimple-domain-security
source_filename: storsimple-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.storsimple.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.storsim'\n  hsts: null\ndomains:\n- domain: storsimple.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storsimple/refs/heads/main/security/storsimple-domain-security.yml
summary_line: DMARC
tags:
- Company
- Storage
- Cloud Storage
- Hybrid Cloud
- Data Management
- Enterprise Storage
- Azure
- Acquired
---
