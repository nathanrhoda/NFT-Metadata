# NFT-Metadata
Some research on NFT and metadata on Opensea

# Intent

Play around with customizing metadata for NFT's


# Setup

1. Setup IPFS
https://docs.ipfs.io/install/command-line/#official-distributions

- Open Powershell
- wget https://dist.ipfs.io/go-ipfs/v0.12.2/go-ipfs_v0.12.2_windows-amd64.zip -Outfile go-ipfs_v0.12.2.zip
- Expand-Archive -Path go-ipfs_v0.12.2.zip -DestinationPath ~\Apps\go-ipfs_v0.12.2
- cd .\go-ipfs_v0.12.2\go-ipfs
- Add path to environment variables
- $GO_IPFS_LOCATION = pwd
- Create Powershell Profile if it doesn't exist "if (!(Test-Path -Path $PROFILE)) { New-Item -ItemType File -Path $PROFILE -Force }"
- notepad $PROFILE
- "Add-Content $PROFILE "`n[System.Environment]::SetEnvironmentVariable('PATH',`$Env:PATH+';;$GO_IPFS_LOCATION')""
- Load Profile  "& $profile"


2. Upload data to ipfs

