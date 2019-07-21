## TestFairy Fetch Sessions tool

Download link: [TestFairy Fetch Sessions](https://github.com/testfairy/testfairy-fetch-sessions/)


### About

This tool downloads screenshots and/or logs from recorded TestFairy sessions. 
Use this to download data you want to analyze with your own toolchain or to import to your own analytics systems.

### Installation

`npm install -g --link git+https://github.com/testfairy/testfairy-fetch-sessions.git`

If you receive the error: "Could not create leading directories", then you should run the same command with `sudo -s` prefix.

### Usage

`testfairy-fetch-sessions --endpoint "acme.testfairy.com" --user "john@example.com" --api-key "0123456789abcdef" --project-id=1000 --logs --screenshots`


The example above would connect to endpoint `acme.testfairy.com` (which can be a private cloud installation, a public cloud installation, or an on-premise installation.) It will use the credentials of `user` and `api-key`.

Since both `--logs` and `--screenshots` are possibble, the tool can download all **screenshots** and all **logs** from app's project 1000. 

You can create an **MP4 video** using all the downloaded screenshots by passing `--video` along with `--screenshots`.

You can find the id of the project (app) you want to download by examining the url (for example: https://app.testfairy.com/projects/1000/).

TestFairy Fetch Sessions tool is incremental in downloads - this means that you can run the tool multiple times, and it will only download new sessions that were recorded.

For Support we're available at [support@testfairy.com](mailto:support@testfairy.com).
