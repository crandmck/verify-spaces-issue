# verify-spaces-issue

Demonstrates issue that Verify truncates the `claim_generator` string after the first space.

This image was signed with c2patool and the `claim_generator` does not contain spaces:
```
    "claim_generator": "C2PA-Tool-test-certs",
```

![](signed-no-spaces.jpg)

This image was signed with c2patool and the `claim_generator` contains spaces:
```
    "claim_generator": "C2PA Tool test certs",
```

![](signed-spaces.jpg)
