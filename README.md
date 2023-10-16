## Running

    npm install --no-fund --no-audit --no-progress --loglevel=error
    npm run shadow-cljs -- -A:cider watch dev

## Problem statement

Despite `-A:cider` being specified, cider-nrepl/refactor-nrepl aren't in the produced classpath (per `ps aux | grep java`),
and trying to connect will visibly show:

    WARNING: CIDER requires cider-nrepl to be fully functional. Some features will not be available without it!
