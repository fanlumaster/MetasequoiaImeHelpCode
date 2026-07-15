# FanImeHelpCode

Helpcodes for [MetasequoiaImeTsf](https://github.com/metasequoiaime/MetasequoiaImeTsf).

For debug:


- helpcode.txt

```powershell
git clone https://github.com/metasequoiaime/MetasequoiaImeHelpCode.git
Remove-Item "C:\Users\<username>\AppData\Local\MetasequoiaImeTsf\helpcode.txt" -Force
New-Item -ItemType SymbolicLink -Path "C:\Users\<username>\AppData\Local\MetasequoiaImeTsf\helpcode.txt" -Target ".\MetasequoiaImeHelpCode\helpcode.txt"
```

- zrm_helpcode_big_unique.txt

```powershell
Remove-Item "C:\Users\<username>\AppData\Local\MetasequoiaImeTsf\zrm_helpcode_big_unique.txt" -Force
New-Item -ItemType SymbolicLink -Path "C:\Users\<username>\AppData\Local\MetasequoiaImeTsf\zrm_helpcode_big_unique.txt" -Target ".\MetasequoiaImeHelpCode\zrm_helpcode_big_unique.txt"
```

e.g.

```powershell
git clone https://github.com/metasequoiaime/MetasequoiaImeHelpCode.git
Remove-Item "C:\Users\SonnyCalcr\AppData\Local\MetasequoiaImeTsf\helpcode.txt" -Force
New-Item -ItemType SymbolicLink -Path "C:\Users\SonnyCalcr\AppData\Local\MetasequoiaImeTsf\helpcode.txt" -Target "C:\Users\SonnyCalcr\EDisk\CppCodes\IMECodes\MetasequoiaImeHelpCode\helpcode.txt"
```

- zrm_helpcode_big_unique.txt

e.g.

```powershell
Remove-Item "C:\Users\SonnyCalcr\AppData\Local\MetasequoiaImeTsf\zrm_helpcode_big_unique" -Force
New-Item -ItemType SymbolicLink -Path "C:\Users\SonnyCalcr\AppData\Local\MetasequoiaImeTsf\zrm_helpcode_big_unique.txt" -Target "C:\Users\SonnyCalcr\EDisk\CppCodes\IMECodes\MetasequoiaImeHelpCode\zrm_helpcode_big_unique.txt"
```

Note: here we must use absolute path.
