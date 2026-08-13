---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cosm.com
  spf: true
- caa: []
  dmarc: true
  dmarc_pct: 20
  dmarc_policy: quarantine
  dmarc_rua: mailto:cosmpostmaster@cosm.com
  dnssec: false
  domain: es.com
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: www.cosm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: tech.cosm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: studios.cosm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: help.cosm.com
  hsts: false
  https: true
  note: Intercom-hosted help center on a Cosm CNAME.
  tls_version: TLSv1.3
- cert_expires: Oct 21 03:21:13 2026 GMT
  host: partners.cosm.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  note: Salesforce Experience Cloud behind Cloudflare; the HSTS is Salesforce's.
  tls_version: TLSv1.3
- cert_expires: Oct 22 22:05:20 2026 GMT
  host: www.es.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: support.es.com
  hsts: false
  http_status: 200
  https: false
  https_error: CERTIFICATE_VERIFY_FAILED - certificate has expired
  note: Linked as the Digistar "Access Portal" from https://tech.cosm.com/products/digistar-projection-system/digistar. https is unusable (expired certificate); http 200 returns a meta-refresh landing page announcing the move to https://partners.cosm.com/.
kind: domain-security
layout: security
method: probed
name: Cosm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosm, probed live across 7 host(s) and 2 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cosm
provider_slug: cosm
slug: cosm-domain-security
source_filename: cosm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Cosm-operated host found on the public site\nnote: >-\n  Cosm publishes no API host, so the probe covers the six web hosts it operates plus\n  the legacy Evans & Sutherland support host. The finding worth flagging is\n  support.es.com — the \"Access Portal\" the Digistar product page still links for\n  documentation and support. Its TLS certificate has EXPIRED, so https fails outright;\n  over plain http it serves an 786-byte meta-refresh to partners.cosm.com. No host\n  outside the Salesforce-operated partner portal sends HSTS, and neither cosm.com nor\n  es.com publishes DNSSEC or CAA.\nhosts:\n- host: www.cosm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: false\n- host: tech.cosm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: false\n- host: studios.cosm.com\n  https: true\n  tls_version: TLSv1.3\n\
  \  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: false\n- host: help.cosm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\n  note: Intercom-hosted help center on a Cosm CNAME.\n- host: partners.cosm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 03:21:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  note: Salesforce Experience Cloud behind Cloudflare; the HSTS is Salesforce's.\n- host: www.es.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 22:05:20 2026 GMT\n  hsts: false\n- host: support.es.com\n  https: false\n  https_error: CERTIFICATE_VERIFY_FAILED - certificate has expired\n  http_status: 200\n  hsts: false\n  note: >-\n    Linked as the Digistar \"Access Portal\" from\n    https://tech.cosm.com/products/digistar-projection-system/digistar. https is\n    unusable (expired certificate); http 200 returns a meta-refresh landing page\n    announcing the move\
  \ to https://partners.cosm.com/.\ndomains:\n- domain: cosm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: es.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 20\n  dmarc_rua: mailto:cosmpostmaster@cosm.com\nx-evidence:\n  fetched: '2026-08-11'\n  hosts_probed: 7\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosm/refs/heads/main/security/cosm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Immersive Experiences
- Entertainment
- Media
- Sports
- Venues
- Display Technology
- Planetarium
- Content Production
---
