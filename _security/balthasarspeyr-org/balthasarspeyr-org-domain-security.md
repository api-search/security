---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: balthasarspeyr.org
  spf: true
hosts:
- cert_expires: Jan 19 11:03:51 2027 GMT
  host: balthasarspeyr.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Balthasarspeyr Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Balthasar & Speyr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Balthasar & Speyr
provider_slug: balthasarspeyr-org
slug: balthasarspeyr-org-domain-security
source_filename: balthasarspeyr-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: balthasarspeyr.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 11:03:51 2027 GMT\n  hsts: false\ndomains:\n- domain: balthasarspeyr.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/balthasarspeyr-org/security/balthasarspeyr-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Theology
- Publications
- Books
- Hans Urs von Balthasar
- Adrienne von Speyr
---
