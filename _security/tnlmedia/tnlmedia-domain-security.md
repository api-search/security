---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tnlmediagene.com
  spf: true
hosts:
- cert_expires: Sep 24 17:07:58 2026 GMT
  host: www.tnlmediagene.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tnlmedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TNL Mediagene, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TNL Mediagene
provider_slug: tnlmedia
slug: tnlmedia-domain-security
source_filename: tnlmedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tnlmediagene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:07:58 2026 GMT\n  hsts: false\ndomains:\n- domain: tnlmediagene.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tnlmedia/refs/heads/main/security/tnlmedia-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Media
- Publishing
- Advertising
- AdTech
- Marketing
- Digital Media
- Content
- Analytics
- E-Commerce
---
