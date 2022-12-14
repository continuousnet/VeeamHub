# VBRJobOptions [Veeam.Backup.Model.CJobOptions]
``` powershell
$job = @(Get-VBRJob | where { $_.JobType -eq "Backup" })[0]
$VBRJobOptions  = Get-VBRJobOptions -job $job
```
* $VBRJobOptions.GetAutoScheduleOptions()  Def [Veeam.Backup.Model.CAutoScheduleOptions GetAutoScheduleOptions(), Veeam.Backup.Model.CAutoScheduleOptions GetAutoScheduleOptions(Veeam.Backup.Model.EDbJobType jobType)]
* $VBRJobOptions.BackupStorageOptions \[Veeam.Backup.Model.CDomBackupStorageOptions\]
* $VBRJobOptions.BackupStorageOptions.TryGetRetainCycles()  Def [System.Nullable[int] TryGetRetainCycles()]
* $VBRJobOptions.BackupStorageOptions.BackupIsAttached \[System.Boolean\]
* $VBRJobOptions.BackupStorageOptions.CheckRetention \[System.Boolean\]
* $VBRJobOptions.BackupStorageOptions.CompressionLevel \[System.Int32\]
* $VBRJobOptions.BackupStorageOptions.EnableDeduplication \[System.Boolean\]
* $VBRJobOptions.BackupStorageOptions.EnableDeletedVmDataRetention \[System.Boolean\]
* $VBRJobOptions.BackupStorageOptions.EnableFullBackup \[System.Boolean\] \($null\)
* $VBRJobOptions.BackupStorageOptions.EnableIntegrityChecks \[System.Boolean\]
* $VBRJobOptions.BackupStorageOptions.KeepFirstFullBackup \[System.Boolean\] \($null\)
* $VBRJobOptions.BackupStorageOptions.RetainCycles \[System.Int32\]
* $VBRJobOptions.BackupStorageOptions.RetainDays \[System.Int32\]
* $VBRJobOptions.BackupStorageOptions.StgBlockSize \[Veeam.Backup.Common.EKbBlockSize\]
* $VBRJobOptions.BackupStorageOptions.StgBlockSize.value__ \[System.Int32\]
* $VBRJobOptions.BackupStorageOptions.StorageEncryptionEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.BackupTargetOptions \[Veeam.Backup.Model.CDomBackupTargetOptions\]
* $VBRJobOptions.BackupTargetOptions.SetTemporaryAlgorithm()  Def [void SetTemporaryAlgorithm(Veeam.Backup.Model.EAlgorithm algorithm)]
* $VBRJobOptions.BackupTargetOptions.Algorithm \[Veeam.Backup.Model.EAlgorithm\]
* $VBRJobOptions.BackupTargetOptions.Algorithm.value__ \[System.Int32\]
* $VBRJobOptions.BackupTargetOptions.FullBackupDays \[System.DayOfWeek[]\]
* $VBRJobOptions.BackupTargetOptions.FullBackupDays.value__ \[System.Int32\]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions \[Veeam.Backup.Model.CDomFullBackupMonthlyScheduleOptions\]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.DayNumberInMonth \[Veeam.Backup.Common.EDayNumberInMonth\]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.DayNumberInMonth.value__ \[System.Int32\]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.DayOfMonth \[Veeam.Backup.Model.CDayOfMonth\]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.DayOfMonth.Build()  Def [string Build()]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.DayOfMonth.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.DayOfMonth.Day \[System.Int32\]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.DayOfMonth.IsLast \[System.Boolean\] \($null\)
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.DayOfMonth.Value \[System.Int32\]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.DayOfWeek \[System.DayOfWeek\]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.DayOfWeek.value__ \[System.Int32\]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.Months \[Veeam.Backup.Common.EMonth[]\]
* $VBRJobOptions.BackupTargetOptions.FullBackupMonthlyScheduleOptions.Months.value__ \[System.Object[]\]
* $VBRJobOptions.BackupTargetOptions.FullBackupScheduleKind \[Veeam.Backup.Model.EFullBackupScheduleKind\] \($null\)
* $VBRJobOptions.BackupTargetOptions.TransformFullToSyntethic \[System.Boolean\] \($null\)
* $VBRJobOptions.BackupTargetOptions.TransformIncrementsToSyntethic \[System.Boolean\] \($null\)
* $VBRJobOptions.BackupTargetOptions.TransformToSyntethicDays \[System.DayOfWeek[]\]
* $VBRJobOptions.BackupTargetOptions.TransformToSyntethicDays.value__ \[System.Int32\]
* $VBRJobOptions.CloudReplicaTargetOptions \[Veeam.Backup.Model.CDomCloudReplicaTargetOptions\]
* $VBRJobOptions.CloudReplicaTargetOptions.CloudConnectHost \[System.Guid\]
* $VBRJobOptions.CloudReplicaTargetOptions.CloudConnectStorage \[System.Guid\]
* $VBRJobOptions.CloudReplicaTargetOptions.ContainerReference \[System.String\] \($null\)
* $VBRJobOptions.EpPolicyOptions \[Veeam.Backup.Model.CDomEpPolicyOptions\]
* $VBRJobOptions.EpPolicyOptions.FindPolicyType()  Def [System.Nullable[Veeam.Backup.Model.EEpPolicyType] FindPolicyType()]
* $VBRJobOptions.EpPolicyOptions.BackupAllUsbDrives \[System.Boolean\] \($null\)
* $VBRJobOptions.EpPolicyOptions.BackupSpecifiedItems \[System.Boolean\] \($null\)
* $VBRJobOptions.EpPolicyOptions.BackupSystemState \[System.Boolean\] \($null\)
* $VBRJobOptions.EpPolicyOptions.BackupUserFolders \[System.Boolean\] \($null\)
* $VBRJobOptions.EpPolicyOptions.DisableBackupOverMeteredConnection \[System.Boolean\] \($null\)
* $VBRJobOptions.EpPolicyOptions.ExcludeMasks \[System.String[]\] \($null\)
* $VBRJobOptions.EpPolicyOptions.IncludeFsItems \[Veeam.Backup.Model.CEpFsItem[]\] \($null\)
* $VBRJobOptions.EpPolicyOptions.IncludeMasks \[System.String[]\] \($null\)
* $VBRJobOptions.EpPolicyOptions.IsSnapshotlessMode \[System.Boolean\] \($null\)
* $VBRJobOptions.EpPolicyOptions.LastReportTime \[$null\] \($null\)
* $VBRJobOptions.EpPolicyOptions.PolicyDestType \[Veeam.Backup.Model.EEpPolicyDestType\] \($null\)
* $VBRJobOptions.EpPolicyOptions.PolicySourceType \[Veeam.Backup.Model.EEpPolicySourceType\] \($null\)
* $VBRJobOptions.EpPolicyOptions.PolicyType \[Veeam.Backup.Model.EEpPolicyType\]
* $VBRJobOptions.EpPolicyOptions.PolicyType.value__ \[System.Int32\]
* $VBRJobOptions.EpPolicyOptions.TargetShareType \[Veeam.Backup.Model.EEpPolicyTargetShareType\] \($null\)
* $VBRJobOptions.EpPolicyOptions.VbrAddress \[System.String\] \($null\)
* $VBRJobOptions.EpPolicyOptions.VbrAuthenticationMode \[Veeam.Backup.Model.EVbrAuthenticationMode\] \($null\)
* $VBRJobOptions.EpPolicyOptions.VbrPort \[System.Int32\]
* $VBRJobOptions.EpPolicyOptions.VbrRetentionType \[System.Boolean\] \($null\)
* $VBRJobOptions.FailoverPlanOptions \[Veeam.Backup.Model.CDomFailoverPlanOptions\]
* $VBRJobOptions.FailoverPlanOptions.PostCommandLine \[System.String\] \($null\)
* $VBRJobOptions.FailoverPlanOptions.PostEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.FailoverPlanOptions.PreCommandLine \[System.String\] \($null\)
* $VBRJobOptions.FailoverPlanOptions.PreEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy \[Veeam.Backup.Model.CDomGenerationPolicy\]
* $VBRJobOptions.GenerationPolicy.CalcGfsPointDateTime()  Def [System.Nullable[datetime] CalcGfsPointDateTime(Veeam.Backup.Model.CStorageInfo+EStorageGFSPeriod period, Veeam.Backup.Common.CDateTimeInterval interval)]
* $VBRJobOptions.GenerationPolicy.GetGFSPointsInPeriod()  Def [Veeam.Backup.Model.CStorageInfo+EStorageGFSPeriod GetGFSPointsInPeriod(Veeam.Backup.Common.CDateTimeInterval interval)]
* $VBRJobOptions.GenerationPolicy.GetNumberOfGfsRetainIntervals()  Def [int GetNumberOfGfsRetainIntervals(Veeam.Backup.Model.CStorageInfo+EStorageGFSPeriod gfsPeriod)]
* $VBRJobOptions.GenerationPolicy.GetPredicateToFindExistedBackup()  Def [System.Func[datetime,bool] GetPredicateToFindExistedBackup(Veeam.Backup.Model.CStorageInfo+EStorageGFSPeriod period, datetime date)]
* $VBRJobOptions.GenerationPolicy.GetPredicateToFindExistedBackupByInterval()  Def [System.Func[Veeam.Backup.Common.CDateTimeInterval,bool] GetPredicateToFindExistedBackupByInterval(Veeam.Backup.Model.CStorageInfo+EStorageGFSPeriod period, datetime date)]
* $VBRJobOptions.GenerationPolicy.GetRpo()  Def [timespan GetRpo()]
* $VBRJobOptions.GenerationPolicy.IntervalAreEquls()  Def [bool IntervalAreEquls(Veeam.Backup.Model.CDateTimeIntervalGFS gfsInterval, Veeam.Backup.Common.CDateTimeInterval interval, Veeam.Backup.Model.CStorageInfo+EStorageGFSPeriod storgePeriods)]
* $VBRJobOptions.GenerationPolicy.IsBackupDate()  Def [bool IsBackupDate(Veeam.Backup.Model.CStorageInfo+EStorageGFSPeriod period, datetime date)]
* $VBRJobOptions.GenerationPolicy.IsFixedSyncIntervalStartTime()  Def [bool IsFixedSyncIntervalStartTime()]
* $VBRJobOptions.GenerationPolicy.IsMonthlyBackupDate()  Def [bool IsMonthlyBackupDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.IsQuarterlyBackupDate()  Def [bool IsQuarterlyBackupDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.IsWeeklyBackupDay()  Def [bool IsWeeklyBackupDay(datetime time)]
* $VBRJobOptions.GenerationPolicy.IsYearlyBackupDate()  Def [bool IsYearlyBackupDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.PickGFSIntervalsByDateInterval()  Def [System.Collections.Generic.IEnumerable[Veeam.Backup.Model.CDateTimeIntervalGFS] PickGFSIntervalsByDateInterval(Veeam.Backup.Common.CDateTimeInterval interval)]
* $VBRJobOptions.GenerationPolicy.WeeklyBackupDateTime()  Def [System.Nullable[datetime] WeeklyBackupDateTime(datetime date), System.Nullable[datetime] WeeklyBackupDateTime(Veeam.Backup.Common.CDateTimeInterval interval)]
* $VBRJobOptions.GenerationPolicy.ActualRetentionRestorePoints \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupDays \[System.DayOfWeek[]\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupDays.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions \[Veeam.Backup.Model.CDomFullBackupMonthlyScheduleOptions\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.DayNumberInMonth \[Veeam.Backup.Common.EDayNumberInMonth\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.DayNumberInMonth.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.DayOfMonth \[Veeam.Backup.Model.CDayOfMonth\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.DayOfMonth.Build()  Def [string Build()]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.DayOfMonth.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.DayOfMonth.Day \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.DayOfMonth.IsLast \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.DayOfMonth.Value \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.DayOfWeek \[System.DayOfWeek\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.DayOfWeek.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.Months \[Veeam.Backup.Common.EMonth[]\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupMonthlyScheduleOptions.Months.value__ \[System.Object[]\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupScheduleKind \[Veeam.Backup.Model.EFullBackupScheduleKind\]
* $VBRJobOptions.GenerationPolicy.CompactFullBackupScheduleKind.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.DailyBackupTime \[System.TimeSpan\]
* $VBRJobOptions.GenerationPolicy.DeletedVmsDataRetentionPeriodDays \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.EnableCompactFull \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy.EnableCompactFullLastTime \[$null\] \($null\)
* $VBRJobOptions.GenerationPolicy.EnableDeletedVmDataRetention \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy.EnableRechek \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy.GFSIsReadEntireRestorePoint \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy.GFSMonthlyBackups \[System.Int32\] \($null\)
* $VBRJobOptions.GenerationPolicy.GFSQuarterlyBackups \[System.Int32\] \($null\)
* $VBRJobOptions.GenerationPolicy.GFSRecentPoints \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.GFSWeeklyBackups \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.GFSYearlyBackups \[System.Int32\] \($null\)
* $VBRJobOptions.GenerationPolicy.IsGfsActiveFullEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy.KeepGfsBackup \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy.MonthlyBackup \[Veeam.Backup.Model.CDomMonthlyBackupCreationTime\]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.BackupDateTime()  Def [datetime BackupDateTime(datetime date)]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.DayOfMonth \[Veeam.Backup.Model.CDayOfMonth\]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.DayOfMonth.Build()  Def [string Build()]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.DayOfMonth.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.DayOfMonth.Day \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.DayOfMonth.IsLast \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.DayOfMonth.Value \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.DayOfWeek \[Veeam.Backup.Model.CDomDayWeek\]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.DayOfWeek.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.DayOfWeek.DayOfWeek \[System.DayOfWeek\] \($null\)
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.DayOfWeek.DayOfWeekNumber \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.Kind \[Veeam.Backup.Model.CDomMonthlyBackupCreationTime+EKind\]
* $VBRJobOptions.GenerationPolicy.MonthlyBackup.Kind.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup \[Veeam.Backup.Model.CDomQuarterlyBackupCreationTime\]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfQuarter \[Veeam.Backup.Model.CDomDayMonth\]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfQuarter.DayNumber \[Veeam.Backup.Model.CDayOfMonth\]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfQuarter.DayNumber.Build()  Def [string Build()]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfQuarter.DayNumber.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfQuarter.DayNumber.Day \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfQuarter.DayNumber.IsLast \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfQuarter.DayNumber.Value \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfQuarter.MonthNumber \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfWeek \[Veeam.Backup.Model.CDomDayWeek\]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfWeek.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfWeek.DayOfWeek \[System.DayOfWeek\] \($null\)
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.DayOfWeek.DayOfWeekNumber \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.Kind \[Veeam.Backup.Model.CDomQuarterlyBackupCreationTime+EKind\]
* $VBRJobOptions.GenerationPolicy.QuarterlyBackup.Kind.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions \[Veeam.Backup.Model.CDomFullBackupMonthlyScheduleOptions\]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.DayNumberInMonth \[Veeam.Backup.Common.EDayNumberInMonth\]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.DayNumberInMonth.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.DayOfMonth \[Veeam.Backup.Model.CDayOfMonth\]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.DayOfMonth.Build()  Def [string Build()]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.DayOfMonth.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.DayOfMonth.Day \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.DayOfMonth.IsLast \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.DayOfMonth.Value \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.DayOfWeek \[System.DayOfWeek\]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.DayOfWeek.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.Months \[Veeam.Backup.Common.EMonth[]\]
* $VBRJobOptions.GenerationPolicy.RecheckBackupMonthlyScheduleOptions.Months.value__ \[System.Object[]\]
* $VBRJobOptions.GenerationPolicy.RecheckDays \[System.DayOfWeek[]\]
* $VBRJobOptions.GenerationPolicy.RecheckDays.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.RecheckScheduleKind \[Veeam.Backup.Model.EFullBackupScheduleKind\]
* $VBRJobOptions.GenerationPolicy.RecheckScheduleKind.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.RecoveryPointObjectiveUnit \[Veeam.Backup.Common.ETimeUnit\]
* $VBRJobOptions.GenerationPolicy.RecoveryPointObjectiveUnit.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.RecoveryPointObjectiveValue \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.RetentionPolicyType \[Veeam.Backup.Model.ERetentionPolicyType\]
* $VBRJobOptions.GenerationPolicy.RetentionPolicyType.value__ \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.SimpleRetentionRestorePoints \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.SyncIntervalStartTime \[System.TimeSpan\]
* $VBRJobOptions.GenerationPolicy.WeeklyBackupDayOfWeek \[System.DayOfWeek\] \($null\)
* $VBRJobOptions.GenerationPolicy.YearlyBackup \[Veeam.Backup.Model.CDomYearlyBackupCreationTime\]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfWeek \[Veeam.Backup.Model.CDomDayWeek\]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfWeek.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfWeek.DayOfWeek \[System.DayOfWeek\] \($null\)
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfWeek.DayOfWeekNumber \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfYear \[Veeam.Backup.Model.CDomDayMonth\]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfYear.DayNumber \[Veeam.Backup.Model.CDayOfMonth\]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfYear.DayNumber.Build()  Def [string Build()]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfYear.DayNumber.MatchDate()  Def [bool MatchDate(datetime date)]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfYear.DayNumber.Day \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfYear.DayNumber.IsLast \[System.Boolean\] \($null\)
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfYear.DayNumber.Value \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.DayOfYear.MonthNumber \[System.Int32\]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.Kind \[Veeam.Backup.Model.CDomYearlyBackupCreationTime+EKind\]
* $VBRJobOptions.GenerationPolicy.YearlyBackup.Kind.value__ \[System.Int32\]
* $VBRJobOptions.HvNetworkMappingOptions \[Veeam.Backup.Model.CDomHvNetworkMappingOptions\]
* $VBRJobOptions.HvNetworkMappingOptions.NetworkMapping \[Veeam.Backup.Model.CHvNetworkMappingSpec[]\] \($null\)
* $VBRJobOptions.HvReplicaTargetOptions \[Veeam.Backup.Model.CDomHvReplicaTargetOptions\]
* $VBRJobOptions.HvReplicaTargetOptions.EnableInitialPass \[System.Boolean\] \($null\)
* $VBRJobOptions.HvReplicaTargetOptions.InitialPassDir \[System.String\] \($null\)
* $VBRJobOptions.HvReplicaTargetOptions.InitialSeeding \[System.Boolean\] \($null\)
* $VBRJobOptions.HvReplicaTargetOptions.ReplicaNameSuffix \[System.String\] \($null\)
* $VBRJobOptions.HvReplicaTargetOptions.TargetFolder \[System.String\]
* $VBRJobOptions.HvReplicaTargetOptions.UseNetworkMapping \[System.Boolean\] \($null\)
* $VBRJobOptions.HvReplicaTargetOptions.UseReIP \[System.Boolean\] \($null\)
* $VBRJobOptions.HvReplicaTargetOptions.UseVmMapping \[System.Boolean\] \($null\)
* $VBRJobOptions.HvSourceOptions \[Veeam.Backup.Model.CDomHvSourceOptions\]
* $VBRJobOptions.HvSourceOptions.CanDoCrashConsistent \[System.Boolean\] \($null\)
* $VBRJobOptions.HvSourceOptions.DirtyBlocksNullingEnabled \[System.Boolean\]
* $VBRJobOptions.HvSourceOptions.EnableHvQuiescence \[System.Boolean\] \($null\)
* $VBRJobOptions.HvSourceOptions.ExcludeSwapFile \[System.Boolean\]
* $VBRJobOptions.HvSourceOptions.FailoverToOnHostBackup \[System.Boolean\]
* $VBRJobOptions.HvSourceOptions.GroupSnapshotProcessing \[System.Boolean\]
* $VBRJobOptions.HvSourceOptions.OffHostBackup \[System.Boolean\]
* $VBRJobOptions.HvSourceOptions.UseChangeTracking \[System.Boolean\]
* $VBRJobOptions.JobOptions \[Veeam.Backup.Model.CDomJobOptions\]
* $VBRJobOptions.JobOptions.BackupCopyJobCanRunAnyTime \[System.Boolean\]
* $VBRJobOptions.JobOptions.RunManually \[System.Boolean\] \($null\)
* $VBRJobOptions.JobOptions.SourceProxyAutoDetect \[System.Boolean\]
* $VBRJobOptions.JobOptions.TargetProxyAutoDetect \[System.Boolean\]
* $VBRJobOptions.JobOptions.ThrottleBackupAgent \[System.Boolean\] \($null\)
* $VBRJobOptions.JobOptions.UseWan \[System.Boolean\] \($null\)
* $VBRJobOptions.JobScriptCommand \[Veeam.Backup.Model.CDomJobScriptCommand\]
* $VBRJobOptions.JobScriptCommand.Serialize()  Def [string Serialize()]
* $VBRJobOptions.JobScriptCommand.Days \[System.DayOfWeek[]\]
* $VBRJobOptions.JobScriptCommand.Days.value__ \[System.Int32\]
* $VBRJobOptions.JobScriptCommand.Frequency \[System.UInt32\]
* $VBRJobOptions.JobScriptCommand.Periodicity \[Veeam.Backup.Model.CDomJobScriptCommand+PeriodicityType\] \($null\)
* $VBRJobOptions.JobScriptCommand.PostCommand \[Veeam.Backup.Model.CCustomCommand\]
* $VBRJobOptions.JobScriptCommand.PostCommand.Clone()  Def [Veeam.Backup.Model.CCustomCommand Clone(), Veeam.Backup.Model.CCustomCommand ICloneable[CCustomCommand].Clone(), System.Object ICloneable.Clone()]
* $VBRJobOptions.JobScriptCommand.PostCommand.CommandLine \[System.String\] \($null\)
* $VBRJobOptions.JobScriptCommand.PostCommand.Days \[System.DayOfWeek[]\]
* $VBRJobOptions.JobScriptCommand.PostCommand.Days.value__ \[System.Int32\]
* $VBRJobOptions.JobScriptCommand.PostCommand.Enabled \[System.Boolean\] \($null\)
* $VBRJobOptions.JobScriptCommand.PostCommand.Frequency \[System.UInt32\]
* $VBRJobOptions.JobScriptCommand.PostCommand.Periodicity \[Veeam.Backup.Model.CCustomCommand+PeriodicityType\] \($null\)
* $VBRJobOptions.JobScriptCommand.PostScriptCommandLine \[System.String\] \($null\)
* $VBRJobOptions.JobScriptCommand.PostScriptEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.JobScriptCommand.PreCommand \[Veeam.Backup.Model.CCustomCommand\]
* $VBRJobOptions.JobScriptCommand.PreCommand.Clone()  Def [Veeam.Backup.Model.CCustomCommand Clone(), Veeam.Backup.Model.CCustomCommand ICloneable[CCustomCommand].Clone(), System.Object ICloneable.Clone()]
* $VBRJobOptions.JobScriptCommand.PreCommand.CommandLine \[System.String\] \($null\)
* $VBRJobOptions.JobScriptCommand.PreCommand.Days \[System.DayOfWeek[]\]
* $VBRJobOptions.JobScriptCommand.PreCommand.Days.value__ \[System.Int32\]
* $VBRJobOptions.JobScriptCommand.PreCommand.Enabled \[System.Boolean\] \($null\)
* $VBRJobOptions.JobScriptCommand.PreCommand.Frequency \[System.UInt32\]
* $VBRJobOptions.JobScriptCommand.PreCommand.Periodicity \[Veeam.Backup.Model.CCustomCommand+PeriodicityType\] \($null\)
* $VBRJobOptions.JobScriptCommand.PreScriptCommandLine \[System.String\] \($null\)
* $VBRJobOptions.JobScriptCommand.PreScriptEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.NotificationOptions \[Veeam.Backup.Model.CDomNotificationOptions\]
* $VBRJobOptions.NotificationOptions.IsResultMatchesJobOptions()  Def [bool IsResultMatchesJobOptions(Veeam.Backup.Model.CBaseSessionInfo+EResult sessResult), bool IJobNotificationOptions.IsResultMatchesJobOptions(Veeam.Backup.Model.CBaseSessionInfo+EResult sessionResult)]
* $VBRJobOptions.NotificationOptions.Serialize()  Def [string Serialize()]
* $VBRJobOptions.NotificationOptions.EmailNotificationAdditionalAddresses \[System.String\] \($null\)
* $VBRJobOptions.NotificationOptions.EmailNotificationSubject \[System.String\]
* $VBRJobOptions.NotificationOptions.EmailNotifyOnError \[System.Boolean\]
* $VBRJobOptions.NotificationOptions.EmailNotifyOnLastRetryOnly \[System.Boolean\]
* $VBRJobOptions.NotificationOptions.EmailNotifyOnSuccess \[System.Boolean\]
* $VBRJobOptions.NotificationOptions.EmailNotifyOnWaitingTape \[System.Boolean\]
* $VBRJobOptions.NotificationOptions.EmailNotifyOnWarning \[System.Boolean\]
* $VBRJobOptions.NotificationOptions.EmailNotifyTime \[System.DateTime\]
* $VBRJobOptions.NotificationOptions.SendEmailNotification2AdditionalAddresses \[System.Boolean\] \($null\)
* $VBRJobOptions.NotificationOptions.SnmpNotification \[System.Boolean\] \($null\)
* $VBRJobOptions.NotificationOptions.UseCustomEmailNotificationOptions \[System.Boolean\] \($null\)
* $VBRJobOptions.Options \[Veeam.Backup.Common.CDomContainer\]
* $VBRJobOptions.Options.Clone()  Def [Veeam.Backup.Common.CDomContainer Clone()]
* $VBRJobOptions.Options.GetObjectData()  Def [void GetObjectData(System.Runtime.Serialization.SerializationInfo info, System.Runtime.Serialization.StreamingContext context), void ISerializable.GetObjectData(System.Runtime.Serialization.SerializationInfo info, System.Runtime.Serialization.StreamingContext context)]
* $VBRJobOptions.Options.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobOptions.Options.Serialize()  Def [string Serialize()]
* $VBRJobOptions.Options.RootNode \[System.Xml.XmlElement\]
* $VBRJobOptions.PolicyOptions \[Veeam.Backup.Model.CDomPolicyOptions\]
* $VBRJobOptions.PolicyOptions.KvpIds \[System.Guid[]\] \($null\)
* $VBRJobOptions.ReIPRulesOptions \[Veeam.Backup.Model.CDomReIPRulesOptions\]
* $VBRJobOptions.ReIPRulesOptions.Add()  Def [Veeam.Backup.Model.CDomReIPRuleOptions Add()]
* $VBRJobOptions.ReIPRulesOptions.Remove()  Def [void Remove(Veeam.Backup.Model.CDomReIPRuleOptions rule)]
* $VBRJobOptions.ReIPRulesOptions.Rules \[Veeam.Backup.Model.CDomReIPRulesOptions+<get_Rules>d__0\] \($null\)
* $VBRJobOptions.ReplicaSourceOptions \[Veeam.Backup.Model.CDomReplicaSourceOptions\]
* $VBRJobOptions.ReplicaSourceOptions.Backup2Vi \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions \[Veeam.Backup.Model.CDomSanIntegrationOptions\]
* $VBRJobOptions.SanIntegrationOptions.DomSanStorageRepositoryOptions \[Veeam.Backup.Model.CDomSanStorageRepositoryOptions\]
* $VBRJobOptions.SanIntegrationOptions.DomSanStorageRepositoryOptions.AddOrUpdateRepository()  Def [void AddOrUpdateRepository(guid repoId, bool isNeedToUse, int retentionCount)]
* $VBRJobOptions.SanIntegrationOptions.DomSanStorageRepositoryOptions.GetRetentionCountByRepository()  Def [int GetRetentionCountByRepository(guid repoId)]
* $VBRJobOptions.SanIntegrationOptions.DomSanStorageRepositoryOptions.HasEnabledRepository()  Def [bool HasEnabledRepository()]
* $VBRJobOptions.SanIntegrationOptions.DomSanStorageRepositoryOptions.IsNeedUseSnapOnlyRepository()  Def [bool IsNeedUseSnapOnlyRepository(guid repoId)]
* $VBRJobOptions.SanIntegrationOptions.DomSanStorageRepositoryOptions.ResetPublicPluginRepositoryOptions()  Def [void ResetPublicPluginRepositoryOptions()]
* $VBRJobOptions.SanIntegrationOptions.Failover2StorageSnapshotBackup \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.FailoverFromSan \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.HpPersistentPeerBackupSource \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.HpPersistentPeerEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.MultipleStorageSnapshotEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.MultipleStorageSnapshotVmsCount \[System.Int32\]
* $VBRJobOptions.SanIntegrationOptions.NimbleSnapshotSourceEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.NimbleSnapshotSourceRetention \[System.Int32\]
* $VBRJobOptions.SanIntegrationOptions.NimbleSnapshotTransferAsBackupSource \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.NimbleSnapshotTransferEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.NimbleSnapshotTransferRetention \[System.Int32\]
* $VBRJobOptions.SanIntegrationOptions.PublicPluginSnapshotSourceEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.PublicPluginSnapshotSourceRetention \[System.Int32\]
* $VBRJobOptions.SanIntegrationOptions.SanSnapshotBackupBackupSource \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.SanSnapshotBackupTransferEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.SanSnapshotBackupTransferRetention \[System.Int32\]
* $VBRJobOptions.SanIntegrationOptions.SanSnapshotReplicaBackupSource \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.SanSnapshotReplicaTransferEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.SanSnapshotReplicaTransferRetention \[System.Int32\]
* $VBRJobOptions.SanIntegrationOptions.SanSnapshotSourceEnabled \[System.Boolean\] \($null\)
* $VBRJobOptions.SanIntegrationOptions.SanSnapshotSourceRetention \[System.Int32\]
* $VBRJobOptions.SanIntegrationOptions.UseSanSnapshots \[System.Boolean\]
* $VBRJobOptions.SqlLogBackupOptions \[Veeam.Backup.Model.CDomSqlLogBackupOptions\]
* $VBRJobOptions.SqlLogBackupOptions.GetBackupInterval()  Def [timespan GetBackupInterval()]
* $VBRJobOptions.SqlLogBackupOptions.GetStorageInterval()  Def [timespan GetStorageInterval()]
* $VBRJobOptions.SqlLogBackupOptions.BackupIntervalUnit \[Veeam.Backup.Common.ETimeUnit\] \($null\)
* $VBRJobOptions.SqlLogBackupOptions.BackupIntervalValue \[System.Int32\]
* $VBRJobOptions.SqlLogBackupOptions.DailyRetentionDays \[System.Int32\]
* $VBRJobOptions.SqlLogBackupOptions.RetentionType \[Veeam.Backup.Model.ESqlLogBackupRetentionType\]
* $VBRJobOptions.SqlLogBackupOptions.RetentionType.value__ \[System.Int32\]
* $VBRJobOptions.SqlLogBackupOptions.StorageIntervalUnit \[Veeam.Backup.Common.ETimeUnit\]
* $VBRJobOptions.SqlLogBackupOptions.StorageIntervalUnit.value__ \[System.Int32\]
* $VBRJobOptions.SqlLogBackupOptions.StorageIntervalValue \[System.Int32\]
* $VBRJobOptions.ViCloudReplicaTargetOptions \[Veeam.Backup.Model.CDomViCloudReplicaTargetOptions\]
* $VBRJobOptions.ViCloudReplicaTargetOptions.CloudConnectDatastore \[System.Guid\]
* $VBRJobOptions.ViCloudReplicaTargetOptions.CloudConnectHost \[System.Guid\]
* $VBRJobOptions.ViCloudReplicaTargetOptions.Enabled \[System.Boolean\] \($null\)
* $VBRJobOptions.ViNetworkMappingOptions \[Veeam.Backup.Model.CDomViNetworkMappingOptions\]
* $VBRJobOptions.ViNetworkMappingOptions.NetworkMapping \[Veeam.Backup.Model.CViNetworkMappingSpec[]\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions \[Veeam.Backup.Model.CDomViReplicaTargetOptions\]
* $VBRJobOptions.ViReplicaTargetOptions.ClusterName \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.ClusterReference \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.DatastoreHDTargetType \[Veeam.Backup.Model.HDTargetType\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.DatastoreName \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.DatastoreReference \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.DatastoreRootPath \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.DiskCreationMode \[Veeam.Backup.Model.EDiskCreationMode\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.EnableDigests \[System.Boolean\]
* $VBRJobOptions.ViReplicaTargetOptions.EnableInitialPass \[System.Boolean\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.HostReference \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.InitialPassDir \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.InitialSeeding \[System.Boolean\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.PbmProfileId \[System.String\]
* $VBRJobOptions.ViReplicaTargetOptions.ReplicaNamePrefix \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.ReplicaNameSuffix \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.ReplicaTargetResourcePoolName \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.ReplicaTargetResourcePoolRef \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.ReplicaTargetVmFolderName \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.ReplicaTargetVmFolderRef \[System.String\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.UseNetworkMapping \[System.Boolean\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.UseReIP \[System.Boolean\] \($null\)
* $VBRJobOptions.ViReplicaTargetOptions.UseVmMapping \[System.Boolean\] \($null\)
* $VBRJobOptions.ViSourceOptions \[Veeam.Backup.Model.CDomViSourceOptions\]
* $VBRJobOptions.ViSourceOptions.GetVCBMode()  Def [Veeam.Backup.Model.VCBModes GetVCBMode()]
* $VBRJobOptions.ViSourceOptions.BackupTemplates \[System.Boolean\]
* $VBRJobOptions.ViSourceOptions.BackupTemplatesOnce \[System.Boolean\]
* $VBRJobOptions.ViSourceOptions.DirtyBlocksNullingEnabled \[System.Boolean\]
* $VBRJobOptions.ViSourceOptions.EnableChangeTracking \[System.Boolean\]
* $VBRJobOptions.ViSourceOptions.EncryptLanTraffic \[System.Boolean\] \($null\)
* $VBRJobOptions.ViSourceOptions.ExcludeSwapFile \[System.Boolean\]
* $VBRJobOptions.ViSourceOptions.FailoverToNetworkMode \[System.Boolean\] \($null\)
* $VBRJobOptions.ViSourceOptions.SetResultsToVmNotes \[System.Boolean\] \($null\)
* $VBRJobOptions.ViSourceOptions.UseChangeTracking \[System.Boolean\]
* $VBRJobOptions.ViSourceOptions.VCBMode \[System.String\]
* $VBRJobOptions.ViSourceOptions.VDDKMode \[System.String\]
* $VBRJobOptions.ViSourceOptions.VmAttributeName \[System.String\]
* $VBRJobOptions.ViSourceOptions.VmNotesAppend \[System.Boolean\]
* $VBRJobOptions.ViSourceOptions.VMToolsQuiesce \[System.Boolean\] \($null\)



