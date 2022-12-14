# VBRJobScheduleOptions [Veeam.Backup.Model.ScheduleOptions]
``` powershell
$job = @(Get-VBRJob | where { $_.JobType -eq "Backup" })[0]
$VBRJobScheduleOptions = Get-VBRJobScheduleOptions -job $job
```
* $VBRJobScheduleOptions.Clone()  Def [Veeam.Backup.Model.ScheduleOptions Clone(), Veeam.Backup.Model.ScheduleOptions ICloneable[ScheduleOptions].Clone(), System.Object ICloneable.Clone()]
* $VBRJobScheduleOptions.DisableEverything()  Def [void DisableEverything()]
* $VBRJobScheduleOptions.FromXmlData()  Def [Veeam.Backup.Model.ScheduleOptions FromXmlData(Veeam.Backup.Common.COutputXmlData data)]
* $VBRJobScheduleOptions.GetDays()  Def [System.DayOfWeek[] GetDays()]
* $VBRJobScheduleOptions.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobScheduleOptions.BackupAtLock \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.BackupAtLogoff \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.BackupAtStartup \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.BackupAtStorageAttach \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.BackupCompetitionWaitingPeriodMin \[System.Int32\]
* $VBRJobScheduleOptions.BackupCompetitionWaitingUnit \[Veeam.Backup.Model.ScheduleOptions+UnitOfTime\]
* $VBRJobScheduleOptions.BackupCompetitionWaitingUnit.value__ \[System.Int32\]
* $VBRJobScheduleOptions.EjectRemovableStorageOnBackupComplete \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.EndDateTimeLocal \[System.DateTime\]
* $VBRJobScheduleOptions.EndDateTimeSpecified \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.FrequencyTimeUnit \[Veeam.Backup.Common.ETimeUnit\]
* $VBRJobScheduleOptions.FrequencyTimeUnit.value__ \[System.Int32\]
* $VBRJobScheduleOptions.IsContinious \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.IsFakeSchedule \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.IsServerMode \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.LatestRecheckLocal \[System.DateTime\]
* $VBRJobScheduleOptions.LatestRunLocal \[System.DateTime\]
* $VBRJobScheduleOptions.LimitBackupsFrequency \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.MaxBackupsFrequency \[System.Int32\]
* $VBRJobScheduleOptions.NextRun \[System.String\]
* $VBRJobScheduleOptions.OptionsBackupWindow \[Veeam.Backup.Model.CBackupWindowOptions\]
* $VBRJobScheduleOptions.OptionsBackupWindow.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobScheduleOptions.OptionsBackupWindow.BackupWindow \[System.String\]
* $VBRJobScheduleOptions.OptionsBackupWindow.IsEnabled \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.OptionsContinuous \[Veeam.Backup.Model.CContinuousOptions\]
* $VBRJobScheduleOptions.OptionsContinuous.GetDays()  Def [System.DayOfWeek[] GetDays()]
* $VBRJobScheduleOptions.OptionsContinuous.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobScheduleOptions.OptionsContinuous.Enabled \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.OptionsContinuous.Schedule \[System.String\]
* $VBRJobScheduleOptions.OptionsDaily \[Veeam.Backup.Model.DailyOptions\]
* $VBRJobScheduleOptions.OptionsDaily.GetDays()  Def [System.DayOfWeek[] GetDays()]
* $VBRJobScheduleOptions.OptionsDaily.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobScheduleOptions.OptionsDaily.CompMode \[Veeam.Backup.Model.ECompMode\] \($null\)
* $VBRJobScheduleOptions.OptionsDaily.DaysSrv \[System.DayOfWeek[]\]
* $VBRJobScheduleOptions.OptionsDaily.DaysSrv.value__ \[System.Object[]\]
* $VBRJobScheduleOptions.OptionsDaily.Enabled \[System.Boolean\]
* $VBRJobScheduleOptions.OptionsDaily.Kind \[Veeam.Backup.Model.DailyOptions+DailyKinds\] \($null\)
* $VBRJobScheduleOptions.OptionsDaily.TimeLocal \[System.DateTime\]
* $VBRJobScheduleOptions.OptionsMonthly \[Veeam.Backup.Model.CMonthlyOptions\]
* $VBRJobScheduleOptions.OptionsMonthly.Clone()  Def [Veeam.Backup.Model.CMonthlyOptions Clone(), Veeam.Backup.Model.CMonthlyOptions ICloneable[CMonthlyOptions].Clone(), System.Object ICloneable.Clone()]
* $VBRJobScheduleOptions.OptionsMonthly.GetDays()  Def [System.DayOfWeek[] GetDays()]
* $VBRJobScheduleOptions.OptionsMonthly.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobScheduleOptions.OptionsMonthly.DayNumberInMonth \[Veeam.Backup.Common.EDayNumberInMonth\]
* $VBRJobScheduleOptions.OptionsMonthly.DayNumberInMonth.value__ \[System.Int32\]
* $VBRJobScheduleOptions.OptionsMonthly.DayOfMonth \[Veeam.Backup.Model.CDayOfMonth\]
* $VBRJobScheduleOptions.OptionsMonthly.DayOfMonth.Build()  Def [string Build()]
* $VBRJobScheduleOptions.OptionsMonthly.DayOfMonth.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobScheduleOptions.OptionsMonthly.DayOfMonth.Day \[System.Int32\]
* $VBRJobScheduleOptions.OptionsMonthly.DayOfMonth.IsLast \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.OptionsMonthly.DayOfMonth.Value \[System.Int32\]
* $VBRJobScheduleOptions.OptionsMonthly.DayOfWeek \[System.DayOfWeek\]
* $VBRJobScheduleOptions.OptionsMonthly.DayOfWeek.value__ \[System.Int32\]
* $VBRJobScheduleOptions.OptionsMonthly.Enabled \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.OptionsMonthly.Months \[Veeam.Backup.Common.EMonth[]\]
* $VBRJobScheduleOptions.OptionsMonthly.Months.value__ \[System.Object[]\]
* $VBRJobScheduleOptions.OptionsMonthly.TimeLocal \[System.DateTime\]
* $VBRJobScheduleOptions.OptionsPeriodically \[Veeam.Backup.Model.PeriodicallyOptions\]
* $VBRJobScheduleOptions.OptionsPeriodically.GetDays()  Def [System.DayOfWeek[] GetDays()]
* $VBRJobScheduleOptions.OptionsPeriodically.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobScheduleOptions.OptionsPeriodically.Enabled \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.OptionsPeriodically.FullPeriod \[System.Int32\]
* $VBRJobScheduleOptions.OptionsPeriodically.HourlyOffset \[System.Int32\] \($null\)
* $VBRJobScheduleOptions.OptionsPeriodically.Kind \[Veeam.Backup.Model.PeriodicallyOptions+PeriodicallyKinds\] \($null\)
* $VBRJobScheduleOptions.OptionsPeriodically.Schedule \[System.String\]
* $VBRJobScheduleOptions.OptionsScheduleAfterJob \[Veeam.Backup.Model.CScheduleAfterJobOptions\]
* $VBRJobScheduleOptions.OptionsScheduleAfterJob.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobScheduleOptions.OptionsScheduleAfterJob.IsEnabled \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.RepeatNumber \[System.Int32\]
* $VBRJobScheduleOptions.RepeatSpecified \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.RepeatTimeUnit \[System.String\]
* $VBRJobScheduleOptions.RepeatTimeUnitMs \[System.Int32\]
* $VBRJobScheduleOptions.ResumeMissedBackup \[System.Boolean\] \($null\)
* $VBRJobScheduleOptions.RetrySpecified \[System.Boolean\]
* $VBRJobScheduleOptions.RetryTimeout \[System.Int32\]
* $VBRJobScheduleOptions.RetryTimes \[System.Int32\]
* $VBRJobScheduleOptions.StartDateTimeLocal \[System.DateTime\]
* $VBRJobScheduleOptions.WaitForBackupCompletion \[System.Boolean\]



