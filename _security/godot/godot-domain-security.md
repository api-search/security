---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: godotengine.org
  spf: true
hosts:
- cert_expires: Oct  7 12:42:53 2026 GMT
  host: godotengine.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 15:28:54 2026 GMT
  host: docs.godotengine.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Godot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Godot Engine, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Godot Engine
provider_slug: godot
slug: godot-domain-security
source_filename: godot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: godotengine.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 12:42:53 2026 GMT\n  hsts: false\n- host: docs.godotengine.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:28:54 2026 GMT\n  hsts: false\ndomains:\n- domain: godotengine.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/godot/refs/heads/main/security/godot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- 2D
- 3D
- C#
- C++
- Game Development
- Game Engine
- GDExtension
- GDScript
- Godot
- Open Source
- Plugin
- SDK
---
