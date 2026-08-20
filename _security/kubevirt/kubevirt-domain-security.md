---
api_specs:
- filename: kubevirt-datasources-api-openapi.yml
  format: yaml
  label: KubeVirt DataSources API
  slug: kubevirt-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/openapi/kubevirt-datasources-api-openapi.yml
- filename: kubevirt-datavolumes-api-openapi.yml
  format: yaml
  label: KubeVirt DataVolumes API
  slug: kubevirt-datavolumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/openapi/kubevirt-datavolumes-api-openapi.yml
- filename: kubevirt-storageprofiles-api-openapi.yml
  format: yaml
  label: KubeVirt StorageProfiles API
  slug: kubevirt-storageprofiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/openapi/kubevirt-storageprofiles-api-openapi.yml
- filename: kubevirt-virtualmachineinstancemigrations-api-openapi.yml
  format: yaml
  label: KubeVirt VirtualMachineInstanceMigrations API
  slug: kubevirt-virtualmachineinstancemigrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/openapi/kubevirt-virtualmachineinstancemigrations-api-openapi.yml
- filename: kubevirt-virtualmachineinstances-api-openapi.yml
  format: yaml
  label: KubeVirt VirtualMachineInstances API
  slug: kubevirt-virtualmachineinstances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/openapi/kubevirt-virtualmachineinstances-api-openapi.yml
- filename: kubevirt-virtualmachines-api-openapi.yml
  format: yaml
  label: KubeVirt VirtualMachines API
  slug: kubevirt-virtualmachines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/openapi/kubevirt-virtualmachines-api-openapi.yml
- filename: kubevirt-vmconsole-api-openapi.yml
  format: yaml
  label: KubeVirt VMConsole API
  slug: kubevirt-vmconsole-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/openapi/kubevirt-vmconsole-api-openapi.yml
- filename: kubevirt-vmlifecycle-api-openapi.yml
  format: yaml
  label: KubeVirt VMLifecycle API
  slug: kubevirt-vmlifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/openapi/kubevirt-vmlifecycle-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kubevirt.io
  spf: false
hosts:
- cert_expires: Sep 20 11:35:21 2026 GMT
  host: kubevirt.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kubevirt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KubeVirt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: KubeVirt
provider_slug: kubevirt
slug: kubevirt-domain-security
source_filename: kubevirt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubevirt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:35:21 2026 GMT\n  hsts: false\ndomains:\n- domain: kubevirt.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/security/kubevirt-domain-security.yml
summary_line: TLSv1.3
tags:
- Cloud-Native
- Incubating
- Kubernetes
- Migration
- Virtual Machines
- Virtualization
---
