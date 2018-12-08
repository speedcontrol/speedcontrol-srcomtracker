# speedcontrol-srcomtracker

This bundle is a helper bundle that gets the donation total/goals/bidwars/new donations from marathon pages on [speedrun.com](https://www.speedrun.com/) if your event has them enabled. It was originally code for [nodecg-speedcontrol](https://github.com/speedcontrol/nodecg-speedcontrol) and is intended to work alongside it, but does not depend on it so could be used for other purposes. Currently undocumented and is subject to change.

### Confg

```
"speedrunComMarathon": {
	"enable": true,
	"slug": "SRC_SLUG"
}
```

Once enabled and a slug is specified of a marathon page on Speedrun.com (this is the part of the URL after the 1st forward slash), if it has donations activated, you will be able to access some information about the marathon's donation information via replicants.
