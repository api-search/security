---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:certs@globality.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: globality.com
  spf: true
hosts:
- cert_expires: Sep 20 04:44:28 2026 GMT
  host: www.globality.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Globality Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Globality, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Globality
provider_slug: globality
slug: globality-domain-security
source_filename: globality-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.globality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:44:28 2026 GMT\n  hsts: false\ndomains:\n- domain: globality.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:certs@globality.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globality/refs/heads/main/security/globality-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Procurement
- Sourcing
- Spend Management
- Artificial Intelligence
- Webhooks
---
