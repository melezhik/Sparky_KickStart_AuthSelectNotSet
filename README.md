# Sparky_KickStart_AuthSelectNotSet

Port authselect-not-set.ks.in  (Test authselect default profile)
to Sparky test

# Report example


```
[task run: task.bash - tasks/test]
[task stdout]
15:00:16 :: test1 /usr/bin/authselect
15:00:16 :: test2 Profile ID: local
15:00:16 :: Enabled features: None
15:00:16 :: 
[task check]
# Test authselect default profile
# authselect is installed
stdout match (w) <test1> True
stdout match (w) </usr/bin/authselect> True
# default authselect configuration is detected
stdout match (w) <test2> True
stdout match (w) <Profile ID: local> True
```

# See also

https://github.com/rhinstaller/kickstart-tests/blob/b3f2e01324fdc2296049054209f94e252b9535d5/authselect-not-set.ks.in
