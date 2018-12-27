# speedcontrol-srcomtracker

This bundle is a helper bundle that gets the donation total/goals/bidwars/new donations from marathon pages on [speedrun.com](https://www.speedrun.com/) if your event has them enabled. It was originally code for [nodecg-speedcontrol](https://github.com/speedcontrol/nodecg-speedcontrol) and is intended to work alongside it, but does not depend on it so could be used for other purposes. Currently (mostly) undocumented and is subject to change.


### Configuration

```
{
	"enable": true,
	"slug": "SRC_SLUG"
}
```

Once enabled and a slug is specified of a marathon page on Speedrun.com (this is the part of the URL after the 1st forward slash), if it has donations activated, you will be able to access some information about the marathon's donation information via replicants.


### Documentation

Due to a lack of decent documentation, here's what was written in the comments of the code that might be able to help you out if you need this bundle:
```
// World's best README, available here:
// Refreshes info from API every 30 seconds.
// Replicants:
//   > donationTotal - current donation total as a float
//   > donationGoals - array of open goals (excluding bidwar related goals)
//   > donationBidwars - array of open bidwars (with embedded goals)
// Messages:
//   > newDonation - donation object (with embedded user/goal/bidwar)
// STILL TO BE ADDED: Prizes (I have no clue how this works yet because no examples)
```