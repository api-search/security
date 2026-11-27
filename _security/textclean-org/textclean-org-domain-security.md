---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: textclean.org
  spf: true
hosts:
- cert_expires: Jan 31 13:08:38 2027 GMT
  host: textclean.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TextClean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TextClean, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TextClean
provider_slug: textclean-org
slug: textclean-org-domain-security
source_filename: textclean-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: textclean.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 13:08:38 2027 GMT\n  hsts: false\ndomains:\n- domain: textclean.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/textclean-org/security/textclean-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- TextCleaning
- BrowserTool
- PrivacyFocused
- Sweden
---
