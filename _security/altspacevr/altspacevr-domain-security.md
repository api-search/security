---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: altvr.com
  spf: false
hosts:
- cert_expires: Oct 12 13:01:39 2026 GMT
  host: altvr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Altspacevr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AltspaceVR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: AltspaceVR
provider_slug: altspacevr
slug: altspacevr-domain-security
source_filename: altspacevr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: altvr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 13:01:39 2026 GMT\n  hsts: false\ndomains:\n- domain: altvr.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altspacevr/refs/heads/main/security/altspacevr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Virtual Reality
- Social VR
- Mixed Reality
- Metaverse
- Gaming
- Discontinued
---
