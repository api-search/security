---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:dgg@axelspace.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: axelspace.com
  spf: true
hosts:
- cert_expires: Nov 30 18:13:23 2026 GMT
  host: www.axelspace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axelspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axelspace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Axelspace
provider_slug: axelspace
slug: axelspace-domain-security
source_filename: axelspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axelspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 18:13:23 2026 GMT\n  hsts: false\ndomains:\n- domain: axelspace.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:dgg@axelspace.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axelspace/refs/heads/main/security/axelspace-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Space
- Satellite
- Imagery
- Data Services
- Innovation
---
