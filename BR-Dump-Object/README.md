# Dumper script as quick powershell reference
## VeeamHub
Veeamhub projects are community driven projects, and are not created by Veeam R&D nor validated by Veeam Q&A. They are maintained by community members which might be or not be Veeam employees. 
## Distributed under MIT license
Copyright (c) 2016 VeeamHub

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Project Notes
**Author:** Timothy Dewin @tdewin

**Function:** Dumps all methods/properties for joboptions and backups

**Requires:** VBR 9.x

**Usage:** Dump-VBRObjects.ps1

**Parameters:** Not Applicable

**Result:** Is actually this file

## QA

**What is this strange syntax @(..)[0]**

The code inside is executed and expected to return an array. For analysis, we only need one object thus we force the return value to be an array and take the first object.

This does mean that you need to have actually one Job defined and have one Backup etc..

# Actual Dump
Using VeeamPSSnapIn v5.1

* [VBRBackup](./VBRBackup.md)
* [VBRBackupPoint](./VBRBackupPoint.md)
* [VBRBackupSession](./VBRBackupSession.md)
* [VBRBackupSessionTaskSession](./VBRBackupSessionTaskSession.md)
* [VBRBackupStorage](./VBRBackupStorage.md)
* [VBRJob](./VBRJob.md)
* [VBRJobObject](./VBRJobObject.md)
* [VBRJobObjectVssOptions](./VBRJobObjectVssOptions.md)
* [VBRJobOptions](./VBRJobOptions.md)
* [VBRJobScheduleOptions](./VBRJobScheduleOptions.md)
* [VBRJobVSSOptions](./VBRJobVSSOptions.md)
* [VBRRestorePoint](./VBRRestorePoint.md)

