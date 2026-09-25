---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bioaegistherapeutics.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Sep 29 08:17:12 2026 GMT
  host: www.bioaegistherapeutics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Bioaegis Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BioAegis Therapeutics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BioAegis Therapeutics
provider_slug: bioaegis-therapeutics
slug: bioaegis-therapeutics-domain-security
source_filename: bioaegis-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bioaegistherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 08:17:12 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: bioaegistherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bioaegis-therapeutics/refs/heads/main/security/bioaegis-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biopharmaceutical
- Biotechnology
- Clinical Trials
- Immunology
- inflammation
- Innate Immunity
- gelsolin
- Protein Therapeutics
- ards
- Critical Care
- Rare Disease
- Drug Development
- Life Sciences
- content-api
---
