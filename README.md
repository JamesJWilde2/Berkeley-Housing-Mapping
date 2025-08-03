# Mapping Downtown Berkeley's planned housing projects

### This project was completed as part of the Lede Program. See the resulting project page [here](https://jamesjwilde2.github.io/berkeley-housing/).

The goal of this project was to find and map all of Downtown Berkeley’s housing projects since the start of 2019. 


## Data collection: 
I pulled data from two main sources.

First, I scraped over 100 meeting minutes [records](https://berkeleyca.gov/your-government/boards-commissions/zoning-adjustments-board) from Berkeley’s Zoning Adjustments Board. I then manually reviewed each record, looking for approved housing projects.

I also reviewed the city’s reports on projects actively under review (accessed via the “reports” button [here](https://aca.cityofberkeley.info/CitizenAccess/Default.aspx)).

I also used [this map](https://www.google.com/maps/d/u/1/viewer?mid=1DAOhWMGII579mvz7sIghdMN-XJWSAOg&ll=37.869524116184046%2C-122.2622703798503&z=16) from Eric Gellerman as initial inspiration and reference. 

I compiled all of this data into one spreadsheet (available in this repo as a csv.)

To define the general boundaries of Downtown Berkeley, I referenced maps from the Downtown Berkeley Association. Two included projects are technically zoned outside of Downtown Berkeley, but I included them because they are roughly included in the Downtown Berkeley map, and because I believe they could plausibly be considered "Downtown Berkeley," which is the point of this map—rather than strictly showing locations within the officially zoned boundaries of Downtown Berkeley. 

**Notes on what I included vs. excluded in the data:**
* Does not include student housing / dorms.
* Does not include building projects that don't include housing.
* Does not include senior housing facilities.
* Does include mixed-used developments that have housing.
* Does not include single family dwellings.
* Does not include special Medak Center theatre housing.
* Only includes new developments—not additions or extensions.
* Only includes projects proposed or approved since the start of 2019 up until May 22, 2025.
* The year the city approved is based on zoning committee approval years. The last date approved in the city's data is listed. Completion dates are based on building permit finaled dates.

## Analysis:
I analyzed the data using a Python notebook available in this repo. Since I created a custom dataset, the actual analysis was relatively straightforward using pandas. 

I also geocoded each address, which I then used to map the data using Datawrapper and Adobe Illustrator. 

## What I learned:
I feel like I barely scratched the surface of what I can do with this analysis, but I’ve already learned a ton about: 
* Scraping websites
* Creating a custom dataset and how tedious it can be
* How time-consuming a full data journalism project can be
* How to clean and structure datasets for use with Datawrapper
* The limits of Datawrapper
* How to use Adobe Illustrator better than a complete beginner
* The importance of setting up GitHub properly to make your life a lot easier


## Future wish list:
There’s a ton that I feel I could add to this project, and I hope to at some point! Some ideas:
* I did my best with creating the custom dataset data, but there are some loose ends I’d like to check up on, including actually visiting each site to verify the state of each project.
* Rather than manually reviewing each minutes document that I scraped, I think I could take advantage of something like Natural PDF next time to extract the data I wanted.
* The project write-up could certainly use some sprucing up.
* I could spend hours and hours refining my maps and visualizations.

And that’s just scratching the surface. Stay tuned!
