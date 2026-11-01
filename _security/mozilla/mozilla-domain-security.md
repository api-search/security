---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:foxsec+caaiodef@mozilla.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mozilla.org
  spf: true
hosts:
- cert_expires: Dec 13 10:07:59 2026 GMT
  host: mozilla.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mozilla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mozilla Glean, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mozilla Glean
provider_slug: mozilla
slug: mozilla-domain-security
source_filename: mozilla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mozilla.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 10:07:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mozilla.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:foxsec+caaiodef@mozilla.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mozilla/security/mozilla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telemetry
- SDK
- OpenSource
- DataEngineering
- Mozilla
---
