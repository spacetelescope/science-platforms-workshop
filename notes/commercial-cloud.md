# Commercial cloud session (2/26/18)

- Pricing models (what’s the deal that STScI have with Amazon?)
  - Essentially zero cost to STScI
  - Worth playing these services off against each other?
  - Co-processing of data is much easier if (Amazon/Google/Microsoft) has it all
- Backups (where, how etc.)
- Vendor lock in
  - Cyverse moves services between vendors (generally different super-computing centers)
  - We should be designing platform-agnostic environments.
  - There is a real cost to move between platforms (perhaps 25% of costs even when using cloud ‘abstractions’ such as K8S)
  - “Do I trust the commercial cloud?”
  - Some assurance that data won’t be lost?
- Service limitations
  - Platform-specific implementations of technologies sometimes aren’t feature-complete
- Data in/out
- Unexpected behaviour (depending upon environment) - e.g. JWST ETC.
- Decadal white paper on co-hosting the data on commodity platforms
  - Focus on software-defined infrastructure?
  - “Don’t just take my code, take my deployable service”
  - Most science projects aren’t able to make good use of commercial cloud without major effort.
- Containers improve the portability of our infrastructure (K8S will be the saviour of astronomy - Frossie) (with minimal overhead)
  - Also lower the cost of managing many smaller services
  - Easier to replace legacy technologies piece-by-piece







