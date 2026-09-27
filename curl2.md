```bash
curl -s -X POST http://localhost:3000/documents/upload/parse \
  -F 'file=@./test-files/02-production-release-sop.pdf' \
  -F 'authorId=10001' \
  -F 'createBy=10001' | jq
```

```bash
DOC_ID='361713143136653312'
curl -s "http://localhost:3000/documents/${DOC_ID}" | jq
```
