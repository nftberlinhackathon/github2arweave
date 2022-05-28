# Github to arweave

MVP Test

```
git clone [...] build
# Skipping CI steps to build
npx arkb deploy ./build --wallet [path to wallet.json]
```

# Actually Production Steps

1. In production, authenticate the user with github oauth
2. Fetch users github repos
3. Let user select the repo
4. Use github api to fetch all the files of the repo
5. Copy the repo and deploy all the files into a build environment using Docker and AWS ECS
6. Produce the build files
7. Send the build files to the frontend
8. Have user login to their AR wallet
9. Create a bundle of the build files and create a transaction with that bundle with arweave.js
10. Have user sign the transaction
11. Pass the URL to the user
12. Site deployed
