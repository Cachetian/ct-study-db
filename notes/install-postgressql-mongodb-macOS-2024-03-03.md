#

Links:

* `https://www.postgresql.org/download/macosx/`
* `https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-os-x/`

Compare

* `https://db-engines.com/en/system/MariaDB;MongoDB;PostgreSQL`

## install PostgresSQL

```shell
❯ brew install postgresql@15


Running `brew update --auto-update`...
==> Auto-updated Homebrew!
==> Updated Homebrew from 4.2.8 (a4ffd6761) to 4.2.10 (53c1107fd).
Updated 1 tap (cloudfoundry/tap).

You have 20 outdated formulae installed.


The 4.2.10 changelog can be found at:
  https://github.com/Homebrew/brew/releases/tag/4.2.10
==> Downloading https://ghcr.io/v2/homebrew/core/postgresql/15/manifests/15.6_1
##################################################################################################################################################################################################### 100.0%
==> Fetching dependencies for postgresql@15: krb5
==> Downloading https://ghcr.io/v2/homebrew/core/krb5/manifests/1.21.2
##################################################################################################################################################################################################### 100.0%
==> Fetching krb5
==> Downloading https://ghcr.io/v2/homebrew/core/krb5/blobs/sha256:2d4dc47f318eb4b612c6082831602dabf86737abaf16205efca110f79d2c4582
##################################################################################################################################################################################################### 100.0%
==> Fetching postgresql@15
==> Downloading https://ghcr.io/v2/homebrew/core/postgresql/15/blobs/sha256:a85110c06097d4cfbc11e0397caf48060d12eac7852556c7eeb99a24885c3fa8
##################################################################################################################################################################################################### 100.0%
==> Installing dependencies for postgresql@15: krb5
==> Installing postgresql@15 dependency: krb5
==> Downloading https://ghcr.io/v2/homebrew/core/krb5/manifests/1.21.2
Already downloaded: /Users/I319998/Library/Caches/Homebrew/downloads/1dac813e15dc58f7f64511565951ee43912a4a82b355448e23600e07b1b7107c--krb5-1.21.2.bottle_manifest.json
==> Pouring krb5--1.21.2.arm64_sonoma.bottle.tar.gz
🍺  /opt/homebrew/Cellar/krb5/1.21.2: 162 files, 5.6MB
==> Installing postgresql@15
==> Pouring postgresql@15--15.6_1.arm64_sonoma.bottle.tar.gz
==> /opt/homebrew/Cellar/postgresql@15/15.6_1/bin/initdb --locale=C -E UTF-8 /opt/homebrew/var/postgresql@15
==> Caveats
This formula has created a default database cluster with:
  initdb --locale=C -E UTF-8 /opt/homebrew/var/postgresql@15
For more details, read:
  https://www.postgresql.org/docs/15/app-initdb.html

postgresql@15 is keg-only, which means it was not symlinked into /opt/homebrew,
because this is an alternate version of another formula.

If you need to have postgresql@15 first in your PATH, run:
  echo 'export PATH="/opt/homebrew/opt/postgresql@15/bin:$PATH"' >> ~/.zshrc

For compilers to find postgresql@15 you may need to set:
  export LDFLAGS="-L/opt/homebrew/opt/postgresql@15/lib"
  export CPPFLAGS="-I/opt/homebrew/opt/postgresql@15/include"

For pkg-config to find postgresql@15 you may need to set:
  export PKG_CONFIG_PATH="/opt/homebrew/opt/postgresql@15/lib/pkgconfig"

To start postgresql@15 now and restart at login:
  brew services start postgresql@15
Or, if you don't want/need a background service you can just run:
  LC_ALL="C" /opt/homebrew/opt/postgresql@15/bin/postgres -D /opt/homebrew/var/postgresql@15
==> Summary
🍺  /opt/homebrew/Cellar/postgresql@15/15.6_1: 3,702 files, 63.1MB
==> Running `brew cleanup postgresql@15`...
Disable this behaviour by setting HOMEBREW_NO_INSTALL_CLEANUP.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).
==> Caveats
==> postgresql@15
This formula has created a default database cluster with:
  initdb --locale=C -E UTF-8 /opt/homebrew/var/postgresql@15
For more details, read:
  https://www.postgresql.org/docs/15/app-initdb.html

postgresql@15 is keg-only, which means it was not symlinked into /opt/homebrew,
because this is an alternate version of another formula.

If you need to have postgresql@15 first in your PATH, run:
  echo 'export PATH="/opt/homebrew/opt/postgresql@15/bin:$PATH"' >> ~/.zshrc

For compilers to find postgresql@15 you may need to set:
  export LDFLAGS="-L/opt/homebrew/opt/postgresql@15/lib"
  export CPPFLAGS="-I/opt/homebrew/opt/postgresql@15/include"

For pkg-config to find postgresql@15 you may need to set:
  export PKG_CONFIG_PATH="/opt/homebrew/opt/postgresql@15/lib/pkgconfig"

To start postgresql@15 now and restart at login:
  brew services start postgresql@15
Or, if you don't want/need a background service you can just run:
  LC_ALL="C" /opt/homebrew/opt/postgresql@15/bin/postgres -D /opt/homebrew/var/postgresql@15
~/GitHub/50-github_com/ct-study-db master
```

## MongoDB

```shell
❯ brew install mongodb-community@7.0
Warning: No available formula with the name "mongodb-community@7.0".
==> Searching for similarly named formulae and casks...
==> Casks
mongodb-compass

To install mongodb-compass, run:
  brew install --cask mongodb-compass
❯ brew update
Already up-to-date.
❯ brew tap mongodb/brew
==> Tapping mongodb/brew
Cloning into '/opt/homebrew/Library/Taps/mongodb/homebrew-brew'...
remote: Enumerating objects: 1324, done.
remote: Counting objects: 100% (373/373), done.
remote: Compressing objects: 100% (90/90), done.
remote: Total 1324 (delta 327), reused 283 (delta 283), pack-reused 951
Receiving objects: 100% (1324/1324), 285.16 KiB | 182.00 KiB/s, done.
Resolving deltas: 100% (765/765), done.
Tapped 17 formulae (35 files, 368.3KB).
❯ brew update
Already up-to-date.
❯ brew install mongodb-community@7.0
==> Fetching dependencies for mongodb/brew/mongodb-community: mongodb/brew/mongodb-database-tools, c-ares, libnghttp2 and mongosh
==> Fetching mongodb/brew/mongodb-database-tools
==> Downloading https://fastdl.mongodb.org/tools/db/mongodb-database-tools-macos-arm64-100.9.4.zip
##################################################################################################################################################################################################### 100.0%
==> Fetching c-ares
==> Downloading https://ghcr.io/v2/homebrew/core/c-ares/manifests/1.27.0
##################################################################################################################################################################################################### 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/c-ares/blobs/sha256:cb6e89367f33ccd46b0971724c9663f329a07d9de4436d645d3240a576a9b469
##################################################################################################################################################################################################### 100.0%
==> Fetching libnghttp2
==> Downloading https://ghcr.io/v2/homebrew/core/libnghttp2/manifests/1.60.0
##################################################################################################################################################################################################### 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/libnghttp2/blobs/sha256:e39f88d586724f1881a69d4126af282eef792632c54895b0a1b70f23cea88479
##################################################################################################################################################################################################### 100.0%
==> Fetching mongosh
==> Downloading https://ghcr.io/v2/homebrew/core/mongosh/manifests/2.1.5
##################################################################################################################################################################################################### 100.0%
==> Downloading https://ghcr.io/v2/homebrew/core/mongosh/blobs/sha256:042b31fb208a5031cde1223098f931bdcd994b9a59e8283f0ce09b13817263d4
##################################################################################################################################################################################################### 100.0%
==> Fetching mongodb/brew/mongodb-community
==> Downloading https://fastdl.mongodb.org/osx/mongodb-macos-arm64-7.0.2.tgz
##################################################################################################################################################################################################### 100.0%
==> Installing mongodb-community from mongodb/brew
Warning: Your Xcode (15.0) is outdated.
Please update to Xcode 15.1 (or delete it).
Xcode can be updated from the App Store.

==> Installing dependencies for mongodb/brew/mongodb-community: mongodb/brew/mongodb-database-tools, c-ares, libnghttp2 and mongosh
==> Installing mongodb/brew/mongodb-community dependency: mongodb/brew/mongodb-database-tools
Warning: Your Xcode (15.0) is outdated.
Please update to Xcode 15.1 (or delete it).
Xcode can be updated from the App Store.

🍺  /opt/homebrew/Cellar/mongodb-database-tools/100.9.4: 13 files, 114.2MB, built in 2 seconds
==> Installing mongodb/brew/mongodb-community dependency: c-ares
==> Downloading https://ghcr.io/v2/homebrew/core/c-ares/manifests/1.27.0
Already downloaded: /Users/I319998/Library/Caches/Homebrew/downloads/701ccb15558e9de47f754a3170d3183a7514532c08d851c7c1dc7f300549b49c--c-ares-1.27.0.bottle_manifest.json
==> Pouring c-ares--1.27.0.arm64_sonoma.bottle.tar.gz
🍺  /opt/homebrew/Cellar/c-ares/1.27.0: 156 files, 1MB
==> Installing mongodb/brew/mongodb-community dependency: libnghttp2
==> Downloading https://ghcr.io/v2/homebrew/core/libnghttp2/manifests/1.60.0
Already downloaded: /Users/I319998/Library/Caches/Homebrew/downloads/93526e3afa1b4f61ef51358f59948495ee0d7dd55c19eba4ca099e969cdc0781--libnghttp2-1.60.0.bottle_manifest.json
==> Pouring libnghttp2--1.60.0.arm64_sonoma.bottle.tar.gz
🍺  /opt/homebrew/Cellar/libnghttp2/1.60.0: 13 files, 808.5KB
==> Installing mongodb/brew/mongodb-community dependency: mongosh
==> Downloading https://ghcr.io/v2/homebrew/core/mongosh/manifests/2.1.5
Already downloaded: /Users/I319998/Library/Caches/Homebrew/downloads/e36cc4d19d415abecec9bf817637ee0973a3f42229f4af06afef43d72f053a1c--mongosh-2.1.5.bottle_manifest.json
==> Pouring mongosh--2.1.5.arm64_sonoma.bottle.tar.gz
Warning: Cask mongodb/brew/mongosh was renamed to homebrew/core/mongosh.
🍺  /opt/homebrew/Cellar/mongosh/2.1.5: 10,707 files, 44.7MB
==> Installing mongodb/brew/mongodb-community
==> Caveats
To start mongodb/brew/mongodb-community now and restart at login:
  brew services start mongodb/brew/mongodb-community
==> Summary
🍺  /opt/homebrew/Cellar/mongodb-community/7.0.2: 11 files, 265.6MB, built in 2 seconds
==> Running `brew cleanup mongodb-community`...
Disable this behaviour by setting HOMEBREW_NO_INSTALL_CLEANUP.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).
==> Upgrading 1 dependent of upgraded formulae:
Disable this behaviour by setting HOMEBREW_NO_INSTALLED_DEPENDENTS_CHECK.
Hide these hints with HOMEBREW_NO_ENV_HINTS (see `man brew`).
unbound 1.19.0 -> 1.19.1
==> Downloading https://ghcr.io/v2/homebrew/core/unbound/manifests/1.19.1
##################################################################################################################################################################################################### 100.0%
==> Checking for dependents of upgraded formulae...
==> No broken dependents found!
==> Caveats
==> mongodb-community
To start mongodb/brew/mongodb-community now and restart at login:
  brew services start mongodb/brew/mongodb-community
~/GitHub/50-github_com/ct-study-db master ?1                                                                                                                                                6m 13s 15:36:26
❯
```
