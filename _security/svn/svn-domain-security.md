---
api_specs:
- filename: svn-webdav-openapi.yml
  format: yaml
  label: SVN WebDAV HTTP API
  slug: svn-webdav-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svn/refs/heads/main/openapi/svn-webdav-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "geotrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sourceforge.io
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: subversion.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 03:36:56 2026 GMT
  host: pysvn.sourceforge.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 19:19:11 2026 GMT
  host: svnkit.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Svn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Subversion, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Subversion
provider_slug: svn
slug: svn-domain-security
source_filename: svn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: subversion.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pysvn.sourceforge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 03:36:56 2026 GMT\n  hsts: false\n- host: svnkit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 19:19:11 2026 GMT\n  hsts: false\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sourceforge.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"geotrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/svn/refs/heads/main/security/svn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache
- Open Source
- Repository
- Source Control
- Svn
- Version Control
- Webdav
---
