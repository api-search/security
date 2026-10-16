---
description: ''
domains:
- caa:
  - 2 iodef "mailto:soc@arbetsformedlingen.se"
  - 1 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "telia.com"
  - 1 iodef "mailto:soc@arbetsformedlingen.se"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: arbetsformedlingen.se
  spf: true
hosts:
- cert_expires: Dec 17 07:06:32 2026 GMT
  host: arbetsformedlingen.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arbetsformedlingen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arbetsförmedlingen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Arbetsförmedlingen
provider_slug: arbetsformedlingen
slug: arbetsformedlingen-domain-security
source_filename: arbetsformedlingen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arbetsformedlingen.se\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 07:06:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arbetsformedlingen.se\n  dnssec: true\n  caa:\n  - 2 iodef \"mailto:soc@arbetsformedlingen.se\"\n  - 1 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"telia.com\"\n  - 1 iodef \"mailto:soc@arbetsformedlingen.se\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arbetsformedlingen/refs/heads/main/security/arbetsformedlingen-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Employment
- Government
- Sweden
- JobSearch
---
