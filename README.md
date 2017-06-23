# VSTS-Release-Report
VSTS Hub Extension to report on cumulative work items associated with builds and releases.

## Problem
In VSTS, Releases are linked to the Builds from which they are created.  Builds are in-turn linked to Changesets which are linked to Work Items that describe the nature of the changes being made in the changeset.  When you create a Release there is a section the defines the assoicated work items.  This can be emailed as a Release Note from the Release view.

In practice however not every build is deployed to an envrionment.  You may have 4 or 5 builds in DEV before you decided to release to TEST.  The Release you create for TEST however only references the latest build and not all the builds since the last release to TEST.  This makes it difficult for the teams to know what Work Items are 'new' in a particular envrionment.

## VSTS Release Report
The VSTS Release Report links these two aspects togther to give a consolodated view of each build, where it has been released and the Work Items associated with each Build.

An user of a particular environment can see when a build was last deployed and the aggregation of work items between each deployment.

![VSTS Release Report](docs/VstsRr1.png)