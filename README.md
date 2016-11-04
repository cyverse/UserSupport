---
layout: page
title: CYVERSE FAQs
---

# Discovery Environment (DE) FAQs

### [Analyses questions](#analyses)

 - [Why has my job failed or been running forever?](#analysesJobFailed)
 - [How do I get help with a tool (app) or workflow?](#analysesHelpToolWorkflow)
 - [Why is my analysis sitting in the Submitted state for so long?](#analysesSubmittedLongTime)
 - [Is there a limit to how many analyses (jobs) I can run at the same time in the Discovery Environment?](#analysesJobLimit)
 - [I’m trying to run an analysis, but when I enter an input I can’t see my files. Why? I know they are there.](#analysesFilesHidden)
 - [How do I rerun a job I previously ran in the DE, but change some parameters or use a different input?](#analysesRelaunch)
 - [How do I run the same analysis on a number of files most efficiently?](#analysesHtFileList)
 - [I have a series of files that need to be analyzed by the same app, but the output files all have the same name. How do I distinguish    them so I can use them in a workflow?](#analysesRenameOutputFiles)

### [Data questions](#data)

 - [How do I share data files and folders in the Discovery Environment?](#dataShare)
 - [When sharing a file or folder, what permission should I give to my collaborator?](#dataPermissions)
 - [Why can’t I rename or delete files in a folder that has been shared with me?](#dataRenameDeleteItem)
 - [How can I manage shared files and folders for my lab group or project?](#dataSharedProject)
 - [Why doesn’t anything happen when I move a folder I own to the trash?](#dataTrashFolder)
 - [Can I have spaces in file and folder names?](#dataSpaces)
 - [Can I view my files in a genome browser?](#dataViewGenome)

### [Apps questions](#apps)

 - [How do I share an app in the Discovery Environment?](#appsDataShareApp)
 - [Why can’t I find a Discovery Environment app?](#appsFindApp)

# ANALYSES
<a name="analyses"></a>

## Why has my job failed or been running forever?
<a name="analysesJobFailed"></a>

[Troubleshooting a Failed Analysis](https://pods.iplantcollaborative.org/wiki/display/DEmanual/Troubleshooting+a+Failed+Analysis) on the CyVerse wiki will help you determine what went wrong and collect information for CyVerse staff in case you cannot resolve the problem yourself.

## How do I get help with a tool (app) or workflow?
<a name="analysesHelpToolWorkflow"></a>

The steps to get help depend on whether you’re a novice or an expert with the tool—executable or binary—on which the app or workflow is based.

#### If you are a novice:

1. **Learn more about the tools used:**

	* Search the internet for the publication describing the tool and any related documentation.

	* Make sure you understand what the tool is designed to do, what inputs it can accept and in which format, and how to set any parameters.

2. **Search the internet for informative sites in your domain.** For example, [SEQanswers](http://seqanswers.com) is the go-to online forum for the next-generation sequencing community.

3. **Talk with someone at your institution** who is more experienced with the tool.

4. **Try to use the app in the Discovery Environment.** Click ![infoicon](docs/images/InfoIcon.jpg) next to the app name to view the app manual and its sample test input files and expected outputs.

5. **Search [Ask CyVerse](http://ask.cyverse.org)** for the answer. If it is not there, post a question.

#### If you are experienced with the tool or workflow:

If you are experienced with the tool or workflow and need advice for how to work with very large-scale data or a complex workflow, you may request community support or [Extended Collaborative Support](http://www.cyverse.org/collaborate).

## Why is my analysis sitting in the Submitted state for so long?
<a name="analysesSubmittedLongTime"></a>

Analyses that use an app that runs on an HPC system can remain in the Submitted state for hours or even days. They may sit in in the queue in Submitted state waiting to run, along with other possibly long-running jobs that were in the queue first. Therefore, it may take several days for your analysis to get its turn to run. Once your analysis runs, its results will be returned to the Data Store and the DE status will change to Completed.

## Is there a limit to how many analyses (jobs) I can run at the same time in the Discovery Environment?
<a name="analysesJobLimit"></a>

Only 8 of your analyses will run at the same time. It’s fine to launch more, but they will not run until some of your analyses have completed.

## I’m trying to run an analysis, but when I enter an input I can’t see my files. Why? I know they are there.
<a name="analysesFilesHidden"></a>

Because the app requires a _folder_ as input, not a _file_, the files don’t show since they aren’t the appropriate inputs for the app. The files are indeed there but don’t show. Check the app’s input box; if it says “Select a folder”, then it requires a folder input. Put the file(s) you want to input into a folder and then use that folder as input. Note: You can use Drag and Drop to input the folder by finding it in the Data window, making sure the folder name is shown in the center panel, and then [dragging](https://wiki.cyverse.org/wiki/display/DEmanual/Moving+a+Data+File+or+Folder#MovingaDataFileorFolder-DragDrop) the folder into the app’s input box.

## How do I rerun a job I previously ran in the DE, but change some parameters or use a different input?
<a name="analysesRelaunch"></a>

You can easily relaunch the same analysis with different settings:

 1. In the Analyses window, click the app name in the App column for the analysis to rerun.
  This opens up an app window for that app, which is already configured with the inputs and settings you used for the previous analysis run.
 2. Change settings or inputs as needed.
 3. Click **Launch Analysis** to launch the new analysis.

[Learn more here.](https://wiki.cyverse.org/wiki/pages/viewpage.action?pageId=11446455#Analyses%20Menu:%20View%20Outputs,%20Parameters,%20and%20Info;%20Relaunch,%20Cancel,%20and%20Delete-Relaunch)

## How do I run the same analysis on a number of files most efficiently?
<a name="analysesHtFileList"></a>

You can create a file that contains a list of up to 16 files to use as input for high-throughput and batch file execution. Such a file is called an HT Analysis Path List file. Learn more [here](https://wiki.cyverse.org/wiki/display/TUT/Parallel+execution%2C+DE+%28Discovery+Environment%29+style), and if you still have questions, read [here](https://pods.iplantcollaborative.org/wiki/display/DEmanual/Creating+New+Files+and+Folders#CreatingNewFilesandFolders-HTanalysispathlist).

## I have a series of files that need to be analyzed by the same app, but the output files all have the same name. How do I distinguish them so I can use them in a workflow?
<a name="analysesRenameOutputFiles"></a>

You can avoid confusion by finding the output folder in your Data list and [renaming](https://wiki.cyverse.org/wiki/display/DEmanual/Renaming+a+Data+File+or+Folder) each output file with a unique name. After renaming the output files, you can then use them together in a step of the analysis workflow.

___

# DATA (FILE & FOLDERS)
<a name="data"></a>

## How do I share data files and folders in the Discovery Environment?
<a name="dataShare"></a>

**To share a file or folder with a CyVerse user:**

 1. Click the checkbox for the file or folder to share.
 2. Click ![shareicon](docs/images/ShareViaDEicon.jpg) in the row for the item.
 3. Begin entering the name in the search field and then select the user.

**To create a public link to a file** (not for folders) with someone who doesn’t have an account:

 1. Click ![linkicon](docs/images/shareviapubliclinkicon.jpg) in the row for the file.
 2. Copy the link, and click **Done**.
 3. Send the link.

Learn more at [Sharing Files and Folders](https://wiki.cyverse.org/wiki/display/DEmanual/Sharing+Files+and+Folders).

## When sharing a file or folder, what permission should I give to my collaborator?
<a name="dataPermissions"></a>

It depends on what you want to allow the collaborator to do with the file or folder. Options are read, write (ability to edit the file or folder), and own (in addition to edit, can also delete and move; use this permission with caution). Learn more [here](https://wiki.cyverse.org/wiki/display/DEmanual/Changing+and+Viewing+Data+Permission+Levels+in+the+DE).

## Why can’t I rename or delete files in a folder that has been shared with me?
<a name="dataRenameDeleteItem"></a>

To rename a file or folder, you must have “write” permission, and to delete a file you must have “own” permission. To check the permission you have, click the checkbox for the item and look at the Permissions shown in the Details panel on the right. Contact the person who shared the file or folder with you if they did not give you the necessary level of permission. Learn more at [Changing and Viewing Data Permission Levels in the DE](https://wiki.cyverse.org/wiki/display/DEmanual/Changing+and+Viewing+Data+Permission+Levels+in+the+DE).

## How can I manage shared files and folders for my lab group or project?
<a name="dataSharedProject"></a>

See [Setting Up a Shared Directory for a Lab or Project](https://wiki.cyverse.org/wiki/display/DC/Setting+up+a+shared+directory+for+a+lab+or+project). **CONTENT NEEDED (RAMONA)**

## Why doesn’t anything happen when I move a folder I own to the trash?
<a name="dataTrashFolder"></a>

If the folder has hundreds of files, it can take several hours for the deletion to complete in the DE. Please be patient and try refreshing your browser periodically. You cannot delete 1000 files or more in the DE. You must [use iCommands](https://wiki.cyverse.org/wiki/display/DS/Using+iCommands) instead. Note that deleted files may still show up in the search for awhile, but eventually will be fully purged from the system.

## Can I have spaces in file and folder names?
<a name="dataSpaces"></a>

Do not use spaces or special characters in file or folder names as they can cause analyses to fail. [Learn more here](https://wiki.cyverse.org/wiki/display/DEmanual/Using+Special+Characters+in+the+DE).

## Can I view my files in a genome browser?
<a name="dataViewGenome"></a>

You can view bam, vcf, and gff genome files you own in the genome browsers at Ensembl, UCSC, IGV, GBrowse, and jbrowse, and view Fasta genome files in CoGe. Learn more about viewing genome files in [a genome browser](https://wiki.cyverse.org/wiki/display/DEmanual/Viewing+Genome+Files+in+a+Genome+Browser) or in  [CoGe](https://pods.iplantcollaborative.org/wiki/display/DEmanual/Viewing+Genome+Files+in+CoGe).

___

# APPS
<a name="apps"></a>

## How do I share an app in the Discovery Environment?
<a name="appsDataShareApp"></a>

You can share an app or workflow with the general public or just with specific users by following the steps described at [Sharing Your App or Workflow and Editing the User Manual](https://wiki.cyverse.org/wiki/display/DEmanual/Sharing+your+App+or+Workflow+and+Editing+the+User+Manual).

## Why can’t I find a Discovery Environment app?
<a name="appsFindApp"></a>

There are two common reasons why an app is not “visible” or doesn’t come up in search in the Apps list:

  * The app may be an HPC (high-performance computing) app, which is only displayed after you have logged in to Agave, where the HPC apps are stored. To do so, click the **HPC** tab in the Apps window and enter your CyVerse username and password.
  * The app may not yet be public, or the app owner may not have shared the unpublished app with you. Check with the owner to see if it is indeed shared with you or public.

If you still can’t find the app, it’s possible it has been deprecated. If an app is no longer returned in a search query, [search](https://wiki.cyverse.org/wiki/display/DEmanual/Searching+for+an+App+or+Workflow#SearchingforanApporWorkflow) for an app with a similar name or one that uses the same tool, topic, or operation. If you are the app integrator and need the app returned to the catalog, contact Support (support@cyverse.org) for assistance. [Learn more about deprecated apps](https://wiki.cyverse.org/wiki/display/DEmanual/Using+the+Apps+Window+and+Submitting+an+Analysis#UsingtheAppsWindowandSubmittinganAnalysis-ArchivedApp).
