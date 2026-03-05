# Sparky_KickStart_AuthSelectNotSet

Port authselect-not-set.ks.in  (Test authselect default profile)
to Sparky test

# Report example


```
[task run: task.bash - tasks/test]
[task stdout]
13:59:36 :: /usr/bin/authselect
13:59:36 :: Profile ID: local
13:59:36 :: Enabled features: None
13:59:36 :: 
[task check]
# Test authselect default profile
# authselect is installed
stdout match (s) </usr/bin/authselect> True
# default authselect configuration is detected"
stdout match (s) <Profile ID: local> True
```

# See also

https://github.com/rhinstaller/kickstart-tests/blob/b3f2e01324fdc2296049054209f94e252b9535d5/authselect-not-set.ks.in
