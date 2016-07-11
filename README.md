# gominer
GPU miner for siacoin in go
Fork of github.com/SiaMining/gominer with poolmod3 patch merged

All available opencl capable GPU's are detected and used in parallel.


## Installation from source

### Prerequisites
* golang (NOT gccgo) version 1.4.2 or above, check with `go version`
* opencl libraries on the library path
* gcc

Ubuntu 14.04 standard repositories only have golang 1.3, so it is recommended
to install version 1.5.1 from the ethereum ppa.

```
add-apt-repository -y ppa:ethereum/ethereum
sudo apt-get update
apt-get install -y git ocl-icd-libopencl1 opencl-headers golang
go get github.com/nerdralph/gominer-nr
```

## Run
```
gominer
```

Usage:
```
  -H string
    	siad host and port (default "localhost:9980")
  -Q string
    	Query string
  -I int
    	Intensity (default 28)
  -E string
        Exclude GPU's: comma separated list of devicenumbers
  -cpu
    	If set, also use the CPU for mining, only GPU's are used by default
  -v	Show version and exit
```

See what intensity gives you the best hashrate.

## FAQ

- *ERROR fetching work - Get http://localhost:9980/miner/headerforwork: dial tcp 127.0.0.1:9980: connection refused*

  Make sure `siad` is running

- What is `siad`?

  Check the sia documentation

- I don't know how to set up siad or the sia UI wallet, how do I do that?

  Check the sia documentation.

- *You have to help me set up mining SIA*

  No I don't

- *Can you log in on my machine to configure my mining setup?*

  No

- I don't know how to get it working, can you help me?

  I get this question at least once a day. Seriously, you can not expect me to set up and support everyone's mining equipment.

- I don't know how to get it working, can you help me please please please ?

  Everyone has his price, make me an offer I can't refuse so I don't have to continue answering `no` to this question.

## Support development

If you really want to, you can support the gominer development:

SIA: 79b9089439218734192db7016f07dc5a0e2a95e873992dd782a1e1306b2c44e116e1d8ded910

BTC: 3QrmVRLU2JZKHiLdATud2vvL9b376wbmKU
