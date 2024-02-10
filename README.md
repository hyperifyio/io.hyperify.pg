**Join our [Discord](https://discord.gg/UBTrHxA78f) to discuss about our software!**

# @heusalagroup/fi.hg.pg

Lightweight PostgreSQL library written in TypeScript.

To use this persister, install following runtime dependencies:

```
npm install --save pg @types/pg
```

See also [hgrs](https://github.com/heusalagroup/hgrs).

### It doesn't have many runtime dependencies

This library expects [@heusalagroup/fi.hg.core](https://github.com/heusalagroup/fi.hg.core) to be located 
in the relative path `../core` and only required dependency it has is for [Lodash 
library](https://lodash.com/).

### We don't have traditional releases

This project evolves directly to our git repository in an agile manner.

This git repository contains only the source code for compile time use case. It is meant to be used 
as a git submodule in a NodeJS or webpack project.

Recommended way to initialize your project is like this:

```
mkdir -p src/fi/hg

git submodule add git@github.com:heusalagroup/fi.hg.core.git src/fi/hg/core
git config -f .gitmodules submodule.src/fi/hg/core.branch main

git submodule add git@github.com:heusalagroup/fi.hg.pg.git src/fi/hg/pg
git config -f .gitmodules submodule.src/fi/hg/pg.branch main
```

Other required dependencies are [the Lodash library](https://lodash.com/) and [pg](https://github.com/brianc/node-postgres):

```
npm install --save-dev lodash @types/lodash pg @types/pg
```

### License

Copyright (c) Heusala Group Ltd. All rights reserved.

Each software release is initially under the HG Evaluation and 
Non-Commercial License for the first two years. This allows use, modification, 
and distribution for non-commercial and evaluation purposes only. Post this 
period, the license transitions to the standard MIT license, permitting broader
usage, including commercial applications. For full details, refer to the 
[LICENSE.md](LICENSE.md) file. 

**Commercial usage licenses can be obtained under separate agreements.**

