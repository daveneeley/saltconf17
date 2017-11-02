**SaltConf 2017 Resources**

Reference cookiecutter formula:
https://github.com/mitodl/saltstack-formula-cookiecutter


/etc/salt/spm.repos.d/artifactory.conf:
```
artifactory_spm:
  url: https://{{ user }}:{{ password }}@{{ artifactory_url }}/artifactory/{{ salt_repo_name }}
```

/etc/salt/master:
```
file_roots:
  base:
    - /srv/salt
    - /srv/spm/salt
```
