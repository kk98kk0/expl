# CVE-2017-1000117
 Malicious Git HTTP Server For CVE-2017-1000117

# 描述
                  This module exploits CVE-2017-1000117, which affects Git
          version 2.7.5 and lower. A submodule of the form 'ssh://' can be passed
          parameters from the username incorrectly. This can be used to inject
          commands to the operating system when the submodule is cloned.
 
          This module creates a fake git repository which contains a submodule
          containing the vulnerability. The vulnerability is triggered when the
          submodules are initialised.

# 测试环境
Start GitLab using:

docker-compose up -d

