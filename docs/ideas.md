Below is a list of project ideas.  You can also find a long list of projects in
previous runs of [CSE
291](https://cseweb.ucsd.edu/~dstefan/cse291-fall16/ideas/) and [CSE
227](https://cseweb.ucsd.edu/classes/sp17/cse227-a/projects.html).  And, of
course, you are welcome to come up with your own ideas.

#### Web related

- Can we [solve :visited once and for all](https://github.com/w3c/csswg-drafts/issues/3012)? How much of the Web will we break if we want to have a same-origin policy for history?
- Revisit browser private modes and evaluate tracking protection mechanisms in modern browsers (e.g., Firefox and Brave).
- Evaluate the effectiveness of Spectre-like timing attacks in deployed, noisy systems.
- Evaluate the security guarantees of out-of-browser HTTP clients (e.g., wget, cURL, and Node.js' HTTP client) especially when compared to modern browser security. Are libraries and applications handling security exceptions (e.g., redirects to HTTP) securely?
- Identify if implicictly-shared state in modern browsers can be used to fingerprint users, leak browsing history, etc.
- Evaluate Site Isolation and Cross-Origin Read Blocking implementations.
- Evaluate the effectiveness of [DeterFox](http://deterfox.com/).
- Implement a boring, secure-by-construction Web framework (e.g., by fleshing out [Frankie](https://github.com/PLSysSec/lio/blob/master/lio-http-server/examples/HelloFrankie.hs)).


#### JavaScript related

- Revisit binding bugs in Node.js and the findbugs in third-party code (the NPM ecosystem).
- Are JavaScript bitcoin wallets (e.g., <https://www.bitaddress.org>) secure?
- Is JavaScript crypto in the wild safe? (Some of the measurements in [CT-Wasm](https://arxiv.org/abs/1808.01348) indicate they may be prone to timing channels.)
- Can we transparently expose SGX to Node.js or browsers (e.g., to allow applications to execute JavaScript code on user data while preserving confidentiality)?

#### Rust related

- Evalute if Rust `unsafe` code in the wild is actually unsafe?
- Are Rust crypto implementations constant-time? Explore macro-based approach to generating constant-time code (much like [FaCT](https://cseweb.ucsd.edu/~dstefan/pubs/cauligi:2017:fact.pdf)).
- Extend [Rocket](https://rocket.rs/) with security enforcement.
- Extend our robust-library sandboxing framework to Rust.

#### Sandboxing related

- Does WebAssembly make it easier to address memory and type safety for legacy, unsafe applications?
- Build a [secure package manager](https://cseweb.ucsd.edu/~dstefan/pubs/brown:2017:spam.pdf), potentially using ML or PL techniques to identify malicious install-time behavior.
- Can we sandbox Haskell install-time and compile-time code? (See [this](https://github.com/haskell/cabal/issues/5303#issuecomment-386758646) for motivation.)
- Measure the effectiveness of off-the-shelf sandboxes (e.g., [FireJail](https://firejail.wordpress.com/)) and their policies?

#### IoT/CPS related

- Extend the [Johnny-Five](http://johnny-five.io/) IoT platform with a safety- and security-enforcement layer.
- Evaluate the security guarantees of an existing IoT or CPS device. For example, [OpenThings](https://openthings.io/), [August lock](https://august.com/), [Dexcom CGM](https://www.dexcom.com/), or Medtronic insulin pump.
- Evaluate the security of building systems or critical city infrastructure.
- Evaluate the security of vehicle-to-vehicle protocols.
