# VBRJobVSSOptions [Veeam.Backup.Model.CGuestProcessingOptions]
``` powershell
$job = @(Get-VBRJob | where { $_.JobType -eq "Backup" })[0]
$VBRJobVSSOptions = Get-VBRJobVSSOptions -job $job
```
* $VBRJobVSSOptions.ApplyAppProcOptions()  Def [void ApplyAppProcOptions(Veeam.Backup.Model.CVssSnapshotOptions vssSnapshotOptions, Veeam.Backup.Model.CSqlBackupOptions sqlBackupOptions, Veeam.Backup.Model.COracleBackupOptions oracleBackupOptions, Veeam.Backup.Model.CSharePointBackupOptions sharePointBackupOptions, Veeam.Backup.Model.CExchangeBackupOptions exchangeBackupOptions, Veeam.Backup.Model.CGuestScriptsOptions scriptsOptions, Veeam.Backup.Model.CGuestFSExcludeOptions guestFSExcludeOptions), void ApplyAppProcOptions(Veeam.Backup.Model.CVssSnapshotOptions vssSnapshotOptions, Veeam.Backup.Model.CSqlBackupOptions sqlBackupOptions, Veeam.Backup.Model.CExchangeBackupOptions exchangeBackupOptions), void ApplyAppProcOptions(Veeam.Backup.Model.CVssSnapshotOptions vssSnapshotOptions), void ApplyAppProcOptions(Veeam.Backup.Model.CVssSnapshotOptions vssSnapshotOptions, Veeam.Backup.Model.CSqlBackupOptions sqlBackupOptions), void ApplyAppProcOptions(Veeam.Backup.Model.CVssSnapshotOptions vssSnapshotOptions, Veeam.Backup.Model.COracleBackupOptions oracleBackupOptions), void ApplyAppProcOptions(Veeam.Backup.Model.CVssSnapshotOptions vssSnapshotOptions, Veeam.Backup.Model.CSharePointBackupOptions sharePointBackupOptions), void ApplyAppProcOptions(Veeam.Backup.Model.CVssSnapshotOptions vssSnapshotOptions, Veeam.Backup.Model.CExchangeBackupOptions exchangeBackupOptions), void ApplyAppProcOptions(Veeam.Backup.Model.CVssSnapshotOptions vssSnapshotOptions, Veeam.Backup.Model.CGuestScriptsOptions scriptsOptions), void ApplyAppProcOptions(Veeam.Backup.Model.CVssSnapshotOptions vssSnapshotOptions, Veeam.Backup.Model.CGuestFSExcludeOptions guestFSExcludeOptions)]
* $VBRJobVSSOptions.ApplyCreds()  Def [void ApplyCreds(guid winCredsId, guid linCredsId)]
* $VBRJobVSSOptions.ApplyGuestFSIndexingOptions()  Def [void ApplyGuestFSIndexingOptions(Veeam.Backup.Model.CGuestFSIndexingOptions winGuestFSIndexingOptions, Veeam.Backup.Model.CGuestFSIndexingOptions linGuestFSIndexingOptions)]
* $VBRJobVSSOptions.Clone()  Def [Veeam.Backup.Model.CGuestProcessingOptions Clone(), Veeam.Backup.Model.CGuestProcessingOptions ICloneable[CGuestProcessingOptions].Clone(), System.Object ICloneable.Clone()]
* $VBRJobVSSOptions.CorrectByPolicyType()  Def [void CorrectByPolicyType(Veeam.Backup.Common.CPlatform platform, Veeam.Backup.Model.EEpPolicyType policyType)]
* $VBRJobVSSOptions.IsBackupOracleRequired()  Def [bool IsBackupOracleRequired()]
* $VBRJobVSSOptions.IsBackupSqlRequired()  Def [bool IsBackupSqlRequired()]
* $VBRJobVSSOptions.IsCustomIndexing()  Def [bool IsCustomIndexing()]
* $VBRJobVSSOptions.IsDontTruncateEnabled()  Def [bool IsDontTruncateEnabled()]
* $VBRJobVSSOptions.IsGuestDbBackupEnabled()  Def [bool IsGuestDbBackupEnabled()]
* $VBRJobVSSOptions.IsGuestFsExcludeOptionsRequired()  Def [bool IsGuestFsExcludeOptionsRequired()]
* $VBRJobVSSOptions.IsIndexingRequired()  Def [bool IsIndexingRequired()]
* $VBRJobVSSOptions.IsLinIndexingRequired()  Def [bool IsLinIndexingRequired()]
* $VBRJobVSSOptions.IsScriptingAllowed()  Def [bool IsScriptingAllowed()]
* $VBRJobVSSOptions.IsScriptingTurnedOn()  Def [bool IsScriptingTurnedOn()]
* $VBRJobVSSOptions.IsSharePointProcessingAllowed()  Def [bool IsSharePointProcessingAllowed()]
* $VBRJobVSSOptions.IsTransactionLogsProcessingAllowed()  Def [bool IsTransactionLogsProcessingAllowed()]
* $VBRJobVSSOptions.IsTruncateSqlAllowed()  Def [bool IsTruncateSqlAllowed()]
* $VBRJobVSSOptions.IsWinIndexingRequired()  Def [bool IsWinIndexingRequired()]
* $VBRJobVSSOptions.ResetLinCreds()  Def [void ResetLinCreds()]
* $VBRJobVSSOptions.ResetLinuxGuestFSCustomIndexing()  Def [void ResetLinuxGuestFSCustomIndexing()]
* $VBRJobVSSOptions.ResetWinCreds()  Def [void ResetWinCreds()]
* $VBRJobVSSOptions.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRJobVSSOptions.Serialize()  Def [string Serialize()]
* $VBRJobVSSOptions.SetScriptingAllowed()  Def [void SetScriptingAllowed()]
* $VBRJobVSSOptions.SetTransactionLogsProcessingAllowed()  Def [void SetTransactionLogsProcessingAllowed()]
* $VBRJobVSSOptions.AreLinCredsSet \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.AreWinCredsSet \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.Enabled \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.ExchangeBackupOptions \[Veeam.Backup.Model.CExchangeBackupOptions\]
* $VBRJobVSSOptions.ExchangeBackupOptions.Apply()  Def [void Apply(Veeam.Backup.Model.CExchangeBackupOptions options)]
* $VBRJobVSSOptions.ExchangeBackupOptions.TransactionLogsProcessing \[Veeam.Backup.Model.ETransactionLogsProcessing\]
* $VBRJobVSSOptions.ExchangeBackupOptions.TransactionLogsProcessing.value__ \[System.Int32\]
* $VBRJobVSSOptions.ExcludedIndexingFolders \[System.String[]\] \($null\)
* $VBRJobVSSOptions.GuestFSExcludeOptions \[Veeam.Backup.Model.CGuestFSExcludeOptions\]
* $VBRJobVSSOptions.GuestFSExcludeOptions.Apply()  Def [void Apply(Veeam.Backup.Model.CGuestFSExcludeOptions options)]
* $VBRJobVSSOptions.GuestFSExcludeOptions.BackupScope \[Veeam.Backup.Model.EGuestFSBackupScope\] \($null\)
* $VBRJobVSSOptions.GuestFSExcludeOptions.ExcludeList \[System.String[]\] \($null\)
* $VBRJobVSSOptions.GuestFSExcludeOptions.FileExcludeEnabled \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.GuestFSExcludeOptions.IncludeList \[System.String[]\] \($null\)
* $VBRJobVSSOptions.GuestFSIndexingType \[Veeam.Backup.Model.EGuestFSIndexingType\] \($null\)
* $VBRJobVSSOptions.GuestProxyAutoDetect \[System.Boolean\]
* $VBRJobVSSOptions.GuestScriptsOptions \[Veeam.Backup.Model.CGuestScriptsOptions\]
* $VBRJobVSSOptions.GuestScriptsOptions.Apply()  Def [void Apply(Veeam.Backup.Model.CGuestScriptsOptions options)]
* $VBRJobVSSOptions.GuestScriptsOptions.CredsId \[System.Guid\]
* $VBRJobVSSOptions.GuestScriptsOptions.IsAtLeastOneScriptSet \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.GuestScriptsOptions.LinScriptFiles \[Veeam.Backup.Model.CScriptFiles\]
* $VBRJobVSSOptions.GuestScriptsOptions.LinScriptFiles.GetPostScriptFilePathWithoutQuotes()  Def [string GetPostScriptFilePathWithoutQuotes()]
* $VBRJobVSSOptions.GuestScriptsOptions.LinScriptFiles.GetPreScriptFilePathWithoutQuotes()  Def [string GetPreScriptFilePathWithoutQuotes()]
* $VBRJobVSSOptions.GuestScriptsOptions.LinScriptFiles.SetInXmlNode()  Def [void SetInXmlNode(System.Xml.XmlNode parentNode, string nodeName)]
* $VBRJobVSSOptions.GuestScriptsOptions.LinScriptFiles.IsAtLeastOneScriptSet \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.GuestScriptsOptions.LinScriptFiles.PostScriptFilePath \[System.String\] \($null\)
* $VBRJobVSSOptions.GuestScriptsOptions.LinScriptFiles.PreScriptFilePath \[System.String\] \($null\)
* $VBRJobVSSOptions.GuestScriptsOptions.ScriptingMode \[Veeam.Backup.Model.EScriptingMode\] \($null\)
* $VBRJobVSSOptions.GuestScriptsOptions.WinScriptFiles \[Veeam.Backup.Model.CScriptFiles\]
* $VBRJobVSSOptions.GuestScriptsOptions.WinScriptFiles.GetPostScriptFilePathWithoutQuotes()  Def [string GetPostScriptFilePathWithoutQuotes()]
* $VBRJobVSSOptions.GuestScriptsOptions.WinScriptFiles.GetPreScriptFilePathWithoutQuotes()  Def [string GetPreScriptFilePathWithoutQuotes()]
* $VBRJobVSSOptions.GuestScriptsOptions.WinScriptFiles.SetInXmlNode()  Def [void SetInXmlNode(System.Xml.XmlNode parentNode, string nodeName)]
* $VBRJobVSSOptions.GuestScriptsOptions.WinScriptFiles.IsAtLeastOneScriptSet \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.GuestScriptsOptions.WinScriptFiles.PostScriptFilePath \[System.String\] \($null\)
* $VBRJobVSSOptions.GuestScriptsOptions.WinScriptFiles.PreScriptFilePath \[System.String\] \($null\)
* $VBRJobVSSOptions.IgnoreErrors \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.IncludedIndexingFolders \[System.String[]\] \($null\)
* $VBRJobVSSOptions.IsFirstUsage \[System.Boolean\]
* $VBRJobVSSOptions.LinCredsId \[System.Guid\]
* $VBRJobVSSOptions.LinExcludedIndexingFolders \[System.String[]\] \($null\)
* $VBRJobVSSOptions.LinGuestFSIndexingOptions \[Veeam.Backup.Model.CGuestFSIndexingOptions\]
* $VBRJobVSSOptions.LinGuestFSIndexingOptions.Apply()  Def [void Apply(Veeam.Backup.Model.CGuestFSIndexingOptions options)]
* $VBRJobVSSOptions.LinGuestFSIndexingOptions.DisableIndexing()  Def [void DisableIndexing()]
* $VBRJobVSSOptions.LinGuestFSIndexingOptions.Enabled \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.LinGuestFSIndexingOptions.ExcludedFolders \[System.String[]\] \($null\)
* $VBRJobVSSOptions.LinGuestFSIndexingOptions.IncludedFolders \[System.String[]\] \($null\)
* $VBRJobVSSOptions.LinGuestFSIndexingOptions.IsIndexingRequired \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.LinGuestFSIndexingOptions.Type \[Veeam.Backup.Model.EGuestFSIndexingType\] \($null\)
* $VBRJobVSSOptions.LinGuestFSIndexingType \[Veeam.Backup.Model.EGuestFSIndexingType\] \($null\)
* $VBRJobVSSOptions.LinIncludedIndexingFolders \[System.String[]\] \($null\)
* $VBRJobVSSOptions.m_isFirstUsage \[System.Boolean\]
* $VBRJobVSSOptions.OracleBackupOptions \[Veeam.Backup.Model.COracleBackupOptions\]
* $VBRJobVSSOptions.OracleBackupOptions.Apply()  Def [void Apply(Veeam.Backup.Model.COracleBackupOptions options)]
* $VBRJobVSSOptions.OracleBackupOptions.DisableBackupLogs()  Def [void DisableBackupLogs()]
* $VBRJobVSSOptions.OracleBackupOptions.DisableProcessing()  Def [void DisableProcessing()]
* $VBRJobVSSOptions.OracleBackupOptions.AccountType \[Veeam.Backup.Model.EOracleAccountType\] \($null\)
* $VBRJobVSSOptions.OracleBackupOptions.ArchivedLogsMaxAgeHours \[System.Int32\]
* $VBRJobVSSOptions.OracleBackupOptions.ArchivedLogsMaxSizeMb \[System.Int32\]
* $VBRJobVSSOptions.OracleBackupOptions.ArchivedLogsTruncation \[Veeam.Backup.Model.EArchivedLogsTruncation\] \($null\)
* $VBRJobVSSOptions.OracleBackupOptions.BackupLogsEnabled \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.OracleBackupOptions.BackupLogsFrequencyMin \[System.Int32\]
* $VBRJobVSSOptions.OracleBackupOptions.ProxyAutoSelect \[System.Boolean\]
* $VBRJobVSSOptions.OracleBackupOptions.RetainDays \[System.Int32\]
* $VBRJobVSSOptions.OracleBackupOptions.SysdbaCredsId \[System.Guid\]
* $VBRJobVSSOptions.OracleBackupOptions.TransactionLogsProcessing \[Veeam.Backup.Model.ETransactionLogsProcessing\] \($null\)
* $VBRJobVSSOptions.OracleBackupOptions.UseDbBackupRetention \[System.Boolean\]
* $VBRJobVSSOptions.SharePointBackupOptions \[Veeam.Backup.Model.CSharePointBackupOptions\]
* $VBRJobVSSOptions.SharePointBackupOptions.Apply()  Def [void Apply(Veeam.Backup.Model.CSharePointBackupOptions options)]
* $VBRJobVSSOptions.SharePointBackupOptions.BackupEnabled \[System.Boolean\]
* $VBRJobVSSOptions.SharePointBackupOptions.CredsId \[System.Guid\]
* $VBRJobVSSOptions.SqlBackupOptions \[Veeam.Backup.Model.CSqlBackupOptions\]
* $VBRJobVSSOptions.SqlBackupOptions.Apply()  Def [void Apply(Veeam.Backup.Model.CSqlBackupOptions options)]
* $VBRJobVSSOptions.SqlBackupOptions.BackupLogsEnabled \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.SqlBackupOptions.BackupLogsFrequencyMin \[System.Int32\]
* $VBRJobVSSOptions.SqlBackupOptions.CredsId \[System.Guid\]
* $VBRJobVSSOptions.SqlBackupOptions.NeverTruncateLogs \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.SqlBackupOptions.ProxyAutoSelect \[System.Boolean\]
* $VBRJobVSSOptions.SqlBackupOptions.RetainDays \[System.Int32\]
* $VBRJobVSSOptions.SqlBackupOptions.TransactionLogsProcessing \[Veeam.Backup.Model.ETransactionLogsProcessing\]
* $VBRJobVSSOptions.SqlBackupOptions.TransactionLogsProcessing.value__ \[System.Int32\]
* $VBRJobVSSOptions.SqlBackupOptions.UseDbBackupRetention \[System.Boolean\]
* $VBRJobVSSOptions.VssSnapshotOptions \[Veeam.Backup.Model.CVssSnapshotOptions\]
* $VBRJobVSSOptions.VssSnapshotOptions.Apply()  Def [void Apply(Veeam.Backup.Model.CVssSnapshotOptions options)]
* $VBRJobVSSOptions.VssSnapshotOptions.ApplicationProcessingEnabled \[System.Boolean\]
* $VBRJobVSSOptions.VssSnapshotOptions.Enabled \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.VssSnapshotOptions.IgnoreErrors \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.VssSnapshotOptions.IsCopyOnly \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.WinCredsId \[System.Guid\]
* $VBRJobVSSOptions.WinGuestFSIndexingOptions \[Veeam.Backup.Model.CGuestFSIndexingOptions\]
* $VBRJobVSSOptions.WinGuestFSIndexingOptions.Apply()  Def [void Apply(Veeam.Backup.Model.CGuestFSIndexingOptions options)]
* $VBRJobVSSOptions.WinGuestFSIndexingOptions.DisableIndexing()  Def [void DisableIndexing()]
* $VBRJobVSSOptions.WinGuestFSIndexingOptions.Enabled \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.WinGuestFSIndexingOptions.ExcludedFolders \[System.String[]\] \($null\)
* $VBRJobVSSOptions.WinGuestFSIndexingOptions.IncludedFolders \[System.String[]\] \($null\)
* $VBRJobVSSOptions.WinGuestFSIndexingOptions.IsIndexingRequired \[System.Boolean\] \($null\)
* $VBRJobVSSOptions.WinGuestFSIndexingOptions.Type \[Veeam.Backup.Model.EGuestFSIndexingType\] \($null\)



