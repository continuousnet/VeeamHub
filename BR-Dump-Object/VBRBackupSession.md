# VBRBackupSession [Veeam.Backup.Core.CBackupSession]
``` powershell
$VBRBackupSession = @(Get-VBRBackupSession | ? {$_.JobType -eq "Backup"})[0]
```
* $VBRBackupSession.AbortSession()  Def [void AbortSession()]
* $VBRBackupSession.CalcBaseSessionResult()  Def [Veeam.Backup.Model.CBaseSessionInfo+EResult CalcBaseSessionResult()]
* $VBRBackupSession.CalcSessionResult()  Def [Veeam.Backup.Model.CBaseSessionInfo+EResult CalcSessionResult()]
* $VBRBackupSession.CanBeEncrypted()  Def [bool CanBeEncrypted(), bool IEncryptedBackupSession.CanBeEncrypted()]
* $VBRBackupSession.CanDelete()  Def [bool CanDelete()]
* $VBRBackupSession.CheckStop()  Def [void CheckStop(), void ISessionStopChecker.CheckStop()]
* $VBRBackupSession.Complete()  Def [void Complete()]
* $VBRBackupSession.CompleteBase()  Def [void CompleteBase()]
* $VBRBackupSession.CompleteUncompletedTasks()  Def [void CompleteUncompletedTasks(System.Exception ex, System.Collections.Generic.IEnumerable[Veeam.Backup.Core.ITask] tasks)]
* $VBRBackupSession.CompleteWithFailure()  Def [void CompleteWithFailure()]
* $VBRBackupSession.CompleteWithResult()  Def [void CompleteWithResult(Veeam.Backup.Model.CBaseSessionInfo+EResult result, Veeam.Backup.Common.ETaskLogRecordStatus status)]
* $VBRBackupSession.CompleteWithSuccess()  Def [void CompleteWithSuccess()]
* $VBRBackupSession.CompleteWithWarning()  Def [void CompleteWithWarning()]
* $VBRBackupSession.CreateNotifyHelper()  Def [Veeam.Backup.Core.CEventNotifier CreateNotifyHelper(System.Nullable[Veeam.Backup.Common.EPlatform] platform, string vmId, string uniqueHash, guid taskSessionId, string objectDisplayName)]
* $VBRBackupSession.CreateTaskSession()  Def [Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom, Veeam.Backup.Core.IXmlLogger logger), Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom), Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, guid objectId, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom), Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, guid objectId, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom, string formattedIpAddress), Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, guid objectId, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom, datetime queuedTime), Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, guid objectId, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom, datetime queuedTime, string formattedIpAddress)]
* $VBRBackupSession.DataBagAddSafe()  Def [void DataBagAddSafe(string key, System.Object value)]
* $VBRBackupSession.DataBagContainsKey()  Def [bool DataBagContainsKey(string key)]
* $VBRBackupSession.DataBagGetOrAddNew()  Def [T DataBagGetOrAddNew[T](string key)]
* $VBRBackupSession.DataBagGetSafe()  Def [T DataBagGetSafe[T](string key, T defaultValue)]
* $VBRBackupSession.FindCreationTimeUtc()  Def [System.Nullable[datetime] FindCreationTimeUtc()]
* $VBRBackupSession.FindEpPolicyContext()  Def [Veeam.Backup.Core.CEpPolicyJobSessionContext FindEpPolicyContext()]
* $VBRBackupSession.FindEpRescanExcludedObjects()  Def [Veeam.Backup.Model.CEpRescanExcludedObjectsInfo FindEpRescanExcludedObjects()]
* $VBRBackupSession.FindJob()  Def [Veeam.Backup.Core.CBackupJob FindJob()]
* $VBRBackupSession.FindJobStartupSpec()  Def [Veeam.Backup.Model.IJobStartupSpec FindJobStartupSpec()]
* $VBRBackupSession.FindObject()  Def [Veeam.Backup.Core.IHierarchyObj FindObject(guid objectId)]
* $VBRBackupSession.FindOrCreateTaskSession()  Def [Veeam.Backup.Core.CBackupTaskSession FindOrCreateTaskSession(string taskSessName, guid objectId, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatform)]
* $VBRBackupSession.FindSessionStarterInfo()  Def [Veeam.Backup.Model.CSessionStarterInfo FindSessionStarterInfo()]
* $VBRBackupSession.FindTaskSession()  Def [Veeam.Backup.Core.CBackupTaskSession FindTaskSession(string taskSessName, guid objectId)]
* $VBRBackupSession.FindTaskSessionByObjectId()  Def [Veeam.Backup.Core.CBackupTaskSession FindTaskSessionByObjectId(guid objectId)]
* $VBRBackupSession.ForceSetDbMethods()  Def [void ForceSetDbMethods(Veeam.Backup.Core.IDbMethodsInterceptor dbMethods)]
* $VBRBackupSession.FreezeEncryptionState()  Def [void FreezeEncryptionState()]
* $VBRBackupSession.GetBackup()  Def [Veeam.Backup.Model.CBackupInfo GetBackup(Veeam.Backup.Core.IDbMethodsInterceptor interceptor), Veeam.Backup.Model.CBackupInfo IDbEncryptionSession.GetBackup(Veeam.Backup.Core.IDbMethodsInterceptor interceptor)]
* $VBRBackupSession.GetBackupStats()  Def [Veeam.Backup.Model.CBackupStats GetBackupStats()]
* $VBRBackupSession.GetChildSessions()  Def [Veeam.Backup.Model.CBackupSessionInfo[] GetChildSessions()]
* $VBRBackupSession.GetDetails()  Def [string GetDetails()]
* $VBRBackupSession.GetFullLogsSubfolder()  Def [Veeam.Backup.Common.CPath GetFullLogsSubfolder(Params string[] children)]
* $VBRBackupSession.GetJob()  Def [Veeam.Backup.Core.CBackupJob GetJob()]
* $VBRBackupSession.GetLastUsedCryptoKey()  Def [Veeam.Backup.Core.CCryptoKey GetLastUsedCryptoKey()]
* $VBRBackupSession.GetOriginalAndRetrySessions()  Def [System.Collections.Generic.IEnumerable[Veeam.Backup.Core.CBackupSession] GetOriginalAndRetrySessions(bool forwardOrdered)]
* $VBRBackupSession.GetRetrySessionModeString()  Def [string GetRetrySessionModeString()]
* $VBRBackupSession.GetTaskSessions()  Def [Veeam.Backup.Core.CBackupTaskSession[] GetTaskSessions()]
* $VBRBackupSession.GetTaskSessionsByStatus()  Def [Veeam.Backup.Core.CBackupTaskSession[] GetTaskSessionsByStatus(Params Veeam.Backup.Model.ESessionStatus[] statuses)]
* $VBRBackupSession.IncrementTotals()  Def [void IncrementTotals(int totalObjects, long totalSize, long totalUsedSize)]
* $VBRBackupSession.IsCloudConnected()  Def [bool IsCloudConnected()]
* $VBRBackupSession.IsPrevOrOriginalSessHaveRecheckError()  Def [bool IsPrevOrOriginalSessHaveRecheckError()]
* $VBRBackupSession.IsSessionNotHeldByJobProcess()  Def [bool IsSessionNotHeldByJobProcess()]
* $VBRBackupSession.IsStoped()  Def [bool IsStoped([ref] string stopDetails), bool IsStoped([ref] string stopDetails, bool bNoLogStopSignal), bool IsStoped(), bool ISessionStopChecker.IsStoped([ref] string stopDetails)]
* $VBRBackupSession.LogAndSetOperation()  Def [void LogAndSetOperation(string format, Params string[] args)]
* $VBRBackupSession.OnSchedulerLoggerCreated()  Def [void OnSchedulerLoggerCreated(Veeam.Backup.Core.CTaskSchedulerSessionLogger taskSchedulerSessionLogger)]
* $VBRBackupSession.ReloadSafe()  Def [void ReloadSafe()]
* $VBRBackupSession.SaveJobProgress()  Def [void SaveJobProgress(), void SaveJobProgress(Veeam.Backup.Common.LogLevels logLevel)]
* $VBRBackupSession.SaveJobProgressExceptObjects()  Def [void SaveJobProgressExceptObjects(Veeam.Backup.Common.LogLevels logLevels)]
* $VBRBackupSession.SaveJobProgressOnlyObjects()  Def [void SaveJobProgressOnlyObjects(Veeam.Backup.Common.LogLevels logLevel)]
* $VBRBackupSession.SendJobFinishEvent()  Def [void SendJobFinishEvent()]
* $VBRBackupSession.SetAuxData()  Def [void SetAuxData(string auxData)]
* $VBRBackupSession.SetDbMethods()  Def [void SetDbMethods(Veeam.Backup.Core.IDbMethodsInterceptor dbMethods)]
* $VBRBackupSession.SetFullMode()  Def [void SetFullMode(bool setActiveFull), void SetFullMode(bool setActiveFull, bool resetPerVmEnabled)]
* $VBRBackupSession.SetLeaseId()  Def [void SetLeaseId(guid leaseId)]
* $VBRBackupSession.SetNonPersistentJob()  Def [void SetNonPersistentJob(Veeam.Backup.Core.CBackupJob job)]
* $VBRBackupSession.SetOperation()  Def [void SetOperation(string format, Params System.Object[] args), void SetOperation(string operation)]
* $VBRBackupSession.SetOriginalSessionId()  Def [void SetOriginalSessionId(guid origSessId)]
* $VBRBackupSession.SetProgress()  Def [void SetProgress(int progress)]
* $VBRBackupSession.SetResult()  Def [void SetResult(Veeam.Backup.Model.CBaseSessionInfo+EResult result), void SetResult(Veeam.Backup.Model.CBaseSessionInfo+EResult result, string resultDescription)]
* $VBRBackupSession.SetRetryPrediction()  Def [void SetRetryPrediction(bool willBeRetried)]
* $VBRBackupSession.SetSpec()  Def [void SetSpec(string spec)]
* $VBRBackupSession.SetState()  Def [void SetState(Veeam.Backup.Model.CBaseSessionInfo+EState state), void IBaseSession.SetState(Veeam.Backup.Model.CBaseSessionInfo+EState state)]
* $VBRBackupSession.SetTotals()  Def [void SetTotals(int totalObjects, long totalSize, long totalUsedSize)]
* $VBRBackupSession.ShouldForceFullBackupByEncriptionEnablingChanging()  Def [bool ShouldForceFullBackupByEncriptionEnablingChanging()]
* $VBRBackupSession.TrySetStateStopping()  Def [bool TrySetStateStopping()]
* $VBRBackupSession.UpdateEpPolicyContext()  Def [void UpdateEpPolicyContext(Veeam.Backup.Core.CEpPolicyJobSessionContext context)]
* $VBRBackupSession.UpdateInnerState()  Def [void UpdateInnerState()]
* $VBRBackupSession.UpdateSessionAlgorithm()  Def [void UpdateSessionAlgorithm(Veeam.Backup.Model.SessionAlgorithms sessionAlgorithm)]
* $VBRBackupSession.UpdateSessionStarterInfo()  Def [void UpdateSessionStarterInfo(Veeam.Backup.Model.CSessionStarterInfo starterInfo)]
* $VBRBackupSession.UpdateStats()  Def [void UpdateStats(Veeam.Backup.Model.CBackupStats stats)]
* $VBRBackupSession.AuxData \[System.String\]
* $VBRBackupSession.BackupStats \[Veeam.Backup.Model.CBackupStats\]
* $VBRBackupSession.BackupStats.GetCompressX()  Def [double GetCompressX()]
* $VBRBackupSession.BackupStats.GetDedupeX()  Def [double GetDedupeX()]
* $VBRBackupSession.BackupStats.SetData()  Def [void SetData(long backupSize, long dataSize, int dedupRatio, int compressRatio)]
* $VBRBackupSession.BackupStats.BackupSize \[System.Int64\]
* $VBRBackupSession.BackupStats.CompressRatio \[System.Int32\]
* $VBRBackupSession.BackupStats.DataSize \[System.Int64\]
* $VBRBackupSession.BackupStats.DedupRatio \[System.Int32\]
* $VBRBackupSession.BackupVerificationResult \[Veeam.Backup.Core.CBackupVerificationResultContainer\]
* $VBRBackupSession.BackupVerificationResult.GetForStorageGroup()  Def [Veeam.Backup.Core.CStorageVerificationResultContainer GetForStorageGroup(guid objectId)]
* $VBRBackupSession.BackupVerificationResult.SetForStorageGroup()  Def [void SetForStorageGroup(guid objectId, System.Collections.Generic.IEnumerable[Veeam.Backup.Core.CStorageVerificationAlg+CStorageVerificationResult] storageVerificationResults)]
* $VBRBackupSession.BaseProgress \[System.Int32\]
* $VBRBackupSession.BottleneckManager \[CJobBottleneckManager\]
* $VBRBackupSession.BottleneckManager.CalcBottleneck()  Def [Veeam.Backup.Model.EBottleneck CalcBottleneck(Veeam.Backup.Model.CBottleneckInfo bottleneckInfo)]
* $VBRBackupSession.BottleneckManager.NetworkThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSession.BottleneckManager.RepositoryReadThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSession.BottleneckManager.RepositoryWriteThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSession.CreationTime \[System.DateTime\]
* $VBRBackupSession.CreationTimeUTC \[System.DateTime\]
* $VBRBackupSession.CurrentPointId \[System.Guid\]
* $VBRBackupSession.DataBag \[System.Collections.Generic.Dictionary`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[System.Object, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\]
* $VBRBackupSession.DataBag.Add()  Def [void Add(string key, System.Object value), void IDictionary[string,Object].Add(string key, System.Object value), void ICollection[KeyValuePair[string,Object]].Add(System.Collections.Generic.KeyValuePair[string,System.Object] item), void IDictionary.Add(System.Object key, System.Object value)]
* $VBRBackupSession.DataBag.Clear()  Def [void Clear(), void ICollection[KeyValuePair[string,Object]].Clear(), void IDictionary.Clear()]
* $VBRBackupSession.DataBag.Contains()  Def [bool ICollection[KeyValuePair[string,Object]].Contains(System.Collections.Generic.KeyValuePair[string,System.Object] item), bool IDictionary.Contains(System.Object key)]
* $VBRBackupSession.DataBag.ContainsKey()  Def [bool ContainsKey(string key), bool IDictionary[string,Object].ContainsKey(string key), bool IReadOnlyDictionary[string,Object].ContainsKey(string key)]
* $VBRBackupSession.DataBag.ContainsValue()  Def [bool ContainsValue(System.Object value)]
* $VBRBackupSession.DataBag.CopyTo()  Def [void ICollection[KeyValuePair[string,Object]].CopyTo(System.Collections.Generic.KeyValuePair[string,System.Object][] array, int arrayIndex), void ICollection.CopyTo(array array, int index)]
* $VBRBackupSession.DataBag.GetEnumerator()  Def [System.Collections.Generic.Dictionary`2+Enumerator[string,System.Object] GetEnumerator(), System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,System.Object]] IEnumerable[KeyValuePair[string,Object]].GetEnumerator(), System.Collections.IEnumerator IEnumerable.GetEnumerator(), System.Collections.IDictionaryEnumerator IDictionary.GetEnumerator()]
* $VBRBackupSession.DataBag.GetObjectData()  Def [void GetObjectData(System.Runtime.Serialization.SerializationInfo info, System.Runtime.Serialization.StreamingContext context), void ISerializable.GetObjectData(System.Runtime.Serialization.SerializationInfo info, System.Runtime.Serialization.StreamingContext context)]
* $VBRBackupSession.DataBag.OnDeserialization()  Def [void OnDeserialization(System.Object sender), void IDeserializationCallback.OnDeserialization(System.Object sender)]
* $VBRBackupSession.DataBag.Remove()  Def [bool Remove(string key), bool IDictionary[string,Object].Remove(string key), bool ICollection[KeyValuePair[string,Object]].Remove(System.Collections.Generic.KeyValuePair[string,System.Object] item), void IDictionary.Remove(System.Object key)]
* $VBRBackupSession.DataBag.TryGetValue()  Def [bool TryGetValue(string key, [ref] System.Object value), bool IDictionary[string,Object].TryGetValue(string key, [ref] System.Object value), bool IReadOnlyDictionary[string,Object].TryGetValue(string key, [ref] System.Object value)]
* $VBRBackupSession.DataBag.Comparer \[System.Collections.Generic.GenericEqualityComparer`1[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\]
* $VBRBackupSession.DataBag.Count \[System.Int32\] \($null\)
* $VBRBackupSession.DataBag.IsFixedSize \[System.Boolean\] \($null\)
* $VBRBackupSession.DataBag.IsReadOnly \[System.Boolean\] \($null\)
* $VBRBackupSession.DataBag.IsSynchronized \[System.Boolean\] \($null\)
* $VBRBackupSession.DataBag.Keys \[System.Collections.Generic.Dictionary`2+KeyCollection[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[System.Object, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSession.DataBag.SyncRoot \[System.Object\]
* $VBRBackupSession.DataBag.Values \[System.Collections.Generic.Dictionary`2+ValueCollection[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[System.Object, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSession.Description \[System.String\] \($null\)
* $VBRBackupSession.EndTime \[System.DateTime\]
* $VBRBackupSession.EndTimeUTC \[System.DateTime\]
* $VBRBackupSession.EventNotifier \[Veeam.Backup.Core.CEventNotifier\]
* $VBRBackupSession.EventNotifier.CompleteSession()  Def [void CompleteSession()]
* $VBRBackupSession.EventNotifier.CreateProgress()  Def [Veeam.Backup.Core.CEventNotifierEntry CreateProgress(Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSession.EventNotifier.Notify()  Def [void Notify(Veeam.Backup.Common.ETaskLogRecordStatus status, Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSession.EventNotifier.NotifySafe()  Def [void NotifySafe(Veeam.Backup.Model.CSessionEventDescriptor descriptor, Veeam.Backup.Model.CSessionEventBinding binding, Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSession.EventNotifier.StartNotifyProgress()  Def [Veeam.Backup.Core.CProgressNotifyHelper StartNotifyProgress(Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSession.Id \[System.Guid\]
* $VBRBackupSession.Info \[Veeam.Backup.Model.CBackupSessionInfo\]
* $VBRBackupSession.Info.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRBackupSession.Info.SetJobAlgorithm()  Def [void SetJobAlgorithm(Veeam.Backup.Model.JobAlgorithms algorithm)]
* $VBRBackupSession.Info.SetSessionAlgorithm()  Def [void SetSessionAlgorithm(Veeam.Backup.Model.SessionAlgorithms algorithm)]
* $VBRBackupSession.Info.AuxData \[System.String\]
* $VBRBackupSession.Info.BackedUpSize \[System.Int64\]
* $VBRBackupSession.Info.BackupTotalSize \[System.Int64\]
* $VBRBackupSession.Info.CompletionPercentage \[System.Int32\]
* $VBRBackupSession.Info.CreationTime \[System.DateTime\]
* $VBRBackupSession.Info.CurrentPointId \[System.Guid\]
* $VBRBackupSession.Info.Description \[System.String\] \($null\)
* $VBRBackupSession.Info.EndTime \[System.DateTime\]
* $VBRBackupSession.Info.Failures \[System.Int32\] \($null\)
* $VBRBackupSession.Info.Id \[System.Guid\]
* $VBRBackupSession.Info.Initiator \[Veeam.Backup.Model.CBaseSessionInfo+SInitiator\]
* $VBRBackupSession.Info.Initiator.Name \[$null\] \($null\)
* $VBRBackupSession.Info.Initiator.Sid \[$null\] \($null\)
* $VBRBackupSession.Info.Initiator2 \[Veeam.Backup.Model.CModifiedUserInfo\]
* $VBRBackupSession.Info.Initiator2.Serialize()  Def [string Serialize(), void Serialize(System.Xml.XmlNode node)]
* $VBRBackupSession.Info.Initiator2.FullName \[System.String\] \($null\)
* $VBRBackupSession.Info.Initiator2.LoginType \[Veeam.Backup.Model.EModifiedUserType\]
* $VBRBackupSession.Info.Initiator2.LoginType.value__ \[System.Int32\]
* $VBRBackupSession.Info.IsActiveFullMode \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.IsCompleted \[System.Boolean\]
* $VBRBackupSession.Info.IsFullMode \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.IsRecheckRetry \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.IsRetryMode \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.IsWorking \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.JobAlgorithm \[Veeam.Backup.Model.JobAlgorithms\]
* $VBRBackupSession.Info.JobAlgorithm.value__ \[System.Int32\]
* $VBRBackupSession.Info.JobId \[System.Guid\]
* $VBRBackupSession.Info.JobName \[System.String\]
* $VBRBackupSession.Info.JobSourceType \[Veeam.Backup.Model.CDbBackupJobInfo+ESourceType\]
* $VBRBackupSession.Info.JobSourceType.value__ \[System.Int32\]
* $VBRBackupSession.Info.JobSpec \[System.String\] \($null\)
* $VBRBackupSession.Info.JobType \[Veeam.Backup.Model.EDbJobType\] \($null\)
* $VBRBackupSession.Info.LeaseId \[System.Guid\]
* $VBRBackupSession.Info.LogsSubFolder \[$null\] \($null\)
* $VBRBackupSession.Info.Operation \[System.String\] \($null\)
* $VBRBackupSession.Info.OriginalSessionId \[System.Guid\]
* $VBRBackupSession.Info.ParentSessionId \[System.Guid\]
* $VBRBackupSession.Info.Platform \[Veeam.Backup.Common.CPlatform\]
* $VBRBackupSession.Info.Platform.IsExternalInfrastructure()  Def [bool IsExternalInfrastructure()]
* $VBRBackupSession.Info.Platform.IsWellKnown()  Def [bool IsWellKnown()]
* $VBRBackupSession.Info.Platform.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRBackupSession.Info.Platform.Platform \[Veeam.Backup.Common.EPlatform\] \($null\)
* $VBRBackupSession.Info.Platform.PlatformId \[System.Guid\]
* $VBRBackupSession.Info.PolicyName \[System.String\] \($null\)
* $VBRBackupSession.Info.PolicyTag \[System.String\] \($null\)
* $VBRBackupSession.Info.Progress \[Veeam.Backup.Model.CBackupProgressData\]
* $VBRBackupSession.Info.Progress.AddChildAndGet()  Def [Veeam.Backup.Model.CBackupProgressData AddChildAndGet(System.Object key, Veeam.Backup.Model.CBackupProgressData child)]
* $VBRBackupSession.Info.Progress.ApplyUpdates()  Def [void ApplyUpdates(Veeam.Backup.Model.CBackupProgressUpdates updates)]
* $VBRBackupSession.Info.Progress.CalcAvgSpeed()  Def [void CalcAvgSpeed()]
* $VBRBackupSession.Info.Progress.CalcPercents()  Def [void CalcPercents()]
* $VBRBackupSession.Info.Progress.Clone()  Def [Veeam.Backup.Model.CBackupProgressData Clone()]
* $VBRBackupSession.Info.Progress.ConvertForeignTimeToLocal()  Def [void ConvertForeignTimeToLocal(timespan timeShift)]
* $VBRBackupSession.Info.Progress.DecrementProcessedSize()  Def [void DecrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSession.Info.Progress.DecrementTotalObjects()  Def [void DecrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSession.Info.Progress.DecrementTotalSize()  Def [void DecrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSession.Info.Progress.FindChild()  Def [Veeam.Backup.Model.CBackupProgressData FindChild(System.Object key)]
* $VBRBackupSession.Info.Progress.GetProcessingDuration()  Def [timespan GetProcessingDuration()]
* $VBRBackupSession.Info.Progress.GetRemainingTime()  Def [timespan GetRemainingTime(System.Nullable[long] avgSpeed)]
* $VBRBackupSession.Info.Progress.IncrementProcessedObjects()  Def [void IncrementProcessedObjects(int deltaProcessedObjects)]
* $VBRBackupSession.Info.Progress.IncrementProcessedSize()  Def [void IncrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSession.Info.Progress.IncrementTotalObjects()  Def [void IncrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSession.Info.Progress.IncrementTotalObjectsWithProcessed()  Def [void IncrementTotalObjectsWithProcessed(int newObjects)]
* $VBRBackupSession.Info.Progress.IncrementTotalSize()  Def [void IncrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSession.Info.Progress.IncrementTotalSizeWithProcessed()  Def [void IncrementTotalSizeWithProcessed(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSession.Info.Progress.RemoveChild()  Def [void RemoveChild(System.Object key)]
* $VBRBackupSession.Info.Progress.Serialize()  Def [string Serialize()]
* $VBRBackupSession.Info.Progress.Start()  Def [void Start()]
* $VBRBackupSession.Info.Progress.Stop()  Def [void Stop(System.Nullable[datetime] stopTime)]
* $VBRBackupSession.Info.Progress.UpdateBottleneck()  Def [void UpdateBottleneck(Veeam.Backup.Model.CBottleneckInfo bottleneckInfo)]
* $VBRBackupSession.Info.Progress.UpdateParentTotalSize()  Def [void UpdateParentTotalSize()]
* $VBRBackupSession.Info.Progress.UpdateParentTotalSizeIfZero()  Def [void UpdateParentTotalSizeIfZero()]
* $VBRBackupSession.Info.Progress.UpdateProcessedObjects()  Def [void UpdateProcessedObjects(int processedObjects)]
* $VBRBackupSession.Info.Progress.UpdateProcessedSize()  Def [void UpdateProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSession.Info.Progress.UpdateTime()  Def [void UpdateTime(datetime startTime, datetime stopTime)]
* $VBRBackupSession.Info.Progress.UpdateTotalObjects()  Def [void UpdateTotalObjects(int totalObjects)]
* $VBRBackupSession.Info.Progress.UpdateTotalSize()  Def [void UpdateTotalSize(long totalSize, long totalUsedSize)]
* $VBRBackupSession.Info.Progress.AvgSpeed \[System.Int64\]
* $VBRBackupSession.Info.Progress.BottleneckInfo \[Veeam.Backup.Model.CBottleneckInfo\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.CalcBottleneck()  Def [Veeam.Backup.Model.EBottleneck CalcBottleneck(bool networkThrottlingEnabled, bool targetRepositoryThrottlingEnabled, bool sourceRepositoryThrottlingEnabled)]
* $VBRBackupSession.Info.Progress.BottleneckInfo.GetSettedValues()  Def [System.Tuple[string,int][] GetSettedValues()]
* $VBRBackupSession.Info.Progress.BottleneckInfo.Serial()  Def [void Serial(System.Xml.XmlNode rootNode)]
* $VBRBackupSession.Info.Progress.BottleneckInfo.Update()  Def [void Update(Veeam.Backup.Model.CBottleneckInfo other)]
* $VBRBackupSession.Info.Progress.BottleneckInfo.Bottleneck \[Veeam.Backup.Model.EBottleneck\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.Bottleneck.value__ \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.Network \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.NetworkThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.Progress.BottleneckInfo.Proxy \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.RepositoryThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.Progress.BottleneckInfo.Source \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.SourceNetwork \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.SourceProxy \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.SourceStorage \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.SourceWan \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.Target \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.TargetNetwork \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.TargetProxy \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.TargetStorage \[System.Int32\]
* $VBRBackupSession.Info.Progress.BottleneckInfo.TargetWan \[System.Int32\]
* $VBRBackupSession.Info.Progress.Duration \[System.TimeSpan\]
* $VBRBackupSession.Info.Progress.IsNeedSubstractReadDelay \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.Progress.Percents \[System.Int32\]
* $VBRBackupSession.Info.Progress.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.ProcessedObjects \[System.Int32\]
* $VBRBackupSession.Info.Progress.ProcessedSize \[System.Int64\]
* $VBRBackupSession.Info.Progress.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.ProcessedUsedSize \[System.Int64\]
* $VBRBackupSession.Info.Progress.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.ReadedAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.ReadedAverageSize \[System.Int64\]
* $VBRBackupSession.Info.Progress.ReadSize \[System.Int64\]
* $VBRBackupSession.Info.Progress.StartTimeLocal \[System.DateTime\]
* $VBRBackupSession.Info.Progress.StartTimeUtc \[System.DateTime\]
* $VBRBackupSession.Info.Progress.StopTimeLocal \[System.DateTime\]
* $VBRBackupSession.Info.Progress.StopTimeUtc \[System.DateTime\]
* $VBRBackupSession.Info.Progress.TotalObjects \[System.Int32\]
* $VBRBackupSession.Info.Progress.TotalSize \[System.Int64\]
* $VBRBackupSession.Info.Progress.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.TotalUsedSize \[System.Int64\]
* $VBRBackupSession.Info.Progress.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.TransferedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.TransferedSize \[System.Int64\]
* $VBRBackupSession.Info.Progress.Updates \[Veeam.Backup.Model.CBackupProgressUpdates\]
* $VBRBackupSession.Info.Progress.Updates.IncrementProcessedDeltas()  Def [void IncrementProcessedDeltas(long processedDeltaIncrement, long processedUsedDeltaIncrement, long readDeltaIncrement, long readAverageDeltaIncrement, long transferredDeltaIncrement)]
* $VBRBackupSession.Info.Progress.Updates.IncrementTotalSizeDeltas()  Def [void IncrementTotalSizeDeltas(long totalSizeDeltaIncrement, long totalUsedSizeDeltaIncrement)]
* $VBRBackupSession.Info.Progress.Updates.Reset()  Def [void Reset()]
* $VBRBackupSession.Info.Progress.Updates.SetChildBottlenecks()  Def [void SetChildBottlenecks(System.Collections.Generic.IDictionary[string,Veeam.Backup.Model.CBottleneckInfo] childBottlenecks)]
* $VBRBackupSession.Info.Progress.Updates.SetChildProcessingIntervals()  Def [void SetChildProcessingIntervals(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Common.CDateTimeInterval][] childIntervals)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks \[System.Collections.Concurrent.ConcurrentDictionary`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.Add()  Def [void IDictionary[string,CBottleneckInfo].Add(string key, Veeam.Backup.Model.CBottleneckInfo value), void ICollection[KeyValuePair[string,CBottleneckInfo]].Add(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Add(System.Object key, System.Object value)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.AddOrUpdate()  Def [Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, Veeam.Backup.Model.CBottleneckInfo addValue, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,TArg,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory, TArg factoryArgument)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.Clear()  Def [void Clear(), void ICollection[KeyValuePair[string,CBottleneckInfo]].Clear(), void IDictionary.Clear()]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.Contains()  Def [bool ICollection[KeyValuePair[string,CBottleneckInfo]].Contains(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), bool IDictionary.Contains(System.Object key)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.ContainsKey()  Def [bool ContainsKey(string key), bool IDictionary[string,CBottleneckInfo].ContainsKey(string key), bool IReadOnlyDictionary[string,CBottleneckInfo].ContainsKey(string key)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.CopyTo()  Def [void ICollection[KeyValuePair[string,CBottleneckInfo]].CopyTo(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo][] array, int arrayIndex), void ICollection.CopyTo(array array, int index)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.GetEnumerator()  Def [System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] GetEnumerator(), System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] IEnumerable[KeyValuePair[string,CBottleneckInfo]].GetEnumerator(), System.Collections.IEnumerator IEnumerable.GetEnumerator(), System.Collections.IDictionaryEnumerator IDictionary.GetEnumerator()]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.GetOrAdd()  Def [Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] valueFactory), Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, Veeam.Backup.Model.CBottleneckInfo value), Veeam.Backup.Model.CBottleneckInfo GetOrAdd[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] valueFactory, TArg factoryArgument)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.Remove()  Def [bool IDictionary[string,CBottleneckInfo].Remove(string key), bool ICollection[KeyValuePair[string,CBottleneckInfo]].Remove(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Remove(System.Object key)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.TryAdd()  Def [bool TryAdd(string key, Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.TryGetValue()  Def [bool TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IReadOnlyDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.TryRemove()  Def [bool TryRemove(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.TryUpdate()  Def [bool TryUpdate(string key, Veeam.Backup.Model.CBottleneckInfo newValue, Veeam.Backup.Model.CBottleneckInfo comparisonValue)]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.Count \[System.Int32\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.IsEmpty \[System.Boolean\]
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.IsFixedSize \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.IsReadOnly \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.IsSynchronized \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.Keys \[System.Collections.ObjectModel.ReadOnlyCollection`1[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.SyncRoot \[$null\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.ChildBottlenecks.Values \[System.Collections.ObjectModel.ReadOnlyCollection`1[[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.ChildProcessingIntervals \[System.Collections.Generic.KeyValuePair`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Common.CDateTimeInterval, Veeam.Backup.Common, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]][]\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.ReadAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.Updates.TransferredDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Info.Progress.UsedSpaceRation \[System.Double\]
* $VBRBackupSession.Info.Result \[Veeam.Backup.Model.CBaseSessionInfo+EResult\] \($null\)
* $VBRBackupSession.Info.RunManually \[System.Boolean\] \($null\)
* $VBRBackupSession.Info.SessionAlgorithm \[Veeam.Backup.Model.SessionAlgorithms\]
* $VBRBackupSession.Info.SessionAlgorithm.value__ \[System.Int32\]
* $VBRBackupSession.Info.State \[Veeam.Backup.Model.CBaseSessionInfo+EState\]
* $VBRBackupSession.Info.State.value__ \[System.Int32\]
* $VBRBackupSession.Info.TransportType \[Veeam.Backup.Model.ETransportType\]
* $VBRBackupSession.Info.TransportType.value__ \[System.Int32\]
* $VBRBackupSession.Info.Warnings \[System.Int32\] \($null\)
* $VBRBackupSession.Info.WillBeRetried \[System.Boolean\] \($null\)
* $VBRBackupSession.IsCompleted \[System.Boolean\]
* $VBRBackupSession.IsEncryptionEnabled \[System.Boolean\] \($null\)
* $VBRBackupSession.IsEncryptionEnabledByOptions \[System.Boolean\] \($null\)
* $VBRBackupSession.IsEpAgentManagement \[System.Boolean\] \($null\)
* $VBRBackupSession.IsFullMode \[System.Boolean\] \($null\)
* $VBRBackupSession.IsLowerAgentPriority \[System.Boolean\]
* $VBRBackupSession.IsManuallyStopped \[System.Boolean\] \($null\)
* $VBRBackupSession.IsPlannedFailover \[System.Boolean\] \($null\)
* $VBRBackupSession.IsPostprocessing \[System.Boolean\] \($null\)
* $VBRBackupSession.IsQuickBackup \[System.Boolean\] \($null\)
* $VBRBackupSession.IsRecheckRetry \[System.Boolean\] \($null\)
* $VBRBackupSession.IsReplicaFromBackup \[System.Boolean\] \($null\)
* $VBRBackupSession.IsRetryMode \[System.Boolean\] \($null\)
* $VBRBackupSession.IsStarting \[System.Boolean\] \($null\)
* $VBRBackupSession.IsTransformLaunched \[System.Boolean\] \($null\)
* $VBRBackupSession.IsVeeamZip \[System.Boolean\] \($null\)
* $VBRBackupSession.IsWorking \[System.Boolean\] \($null\)
* $VBRBackupSession.JobId \[System.Guid\]
* $VBRBackupSession.JobName \[System.String\]
* $VBRBackupSession.JobSourceType \[Veeam.Backup.Model.CDbBackupJobInfo+ESourceType\]
* $VBRBackupSession.JobSourceType.value__ \[System.Int32\]
* $VBRBackupSession.JobSpec \[System.String\] \($null\)
* $VBRBackupSession.JobType \[Veeam.Backup.Model.EDbJobType\] \($null\)
* $VBRBackupSession.JobTypeString \[System.String\]
* $VBRBackupSession.LastProgressSaveTime \[System.DateTime\]
* $VBRBackupSession.LeaseId \[System.Guid\]
* $VBRBackupSession.Logger \[Veeam.Backup.Core.XmlLogger\]
* $VBRBackupSession.Logger.AddErr()  Def [uint64 AddErr(System.Exception exception, string title, Params System.Object[] args), uint64 AddErr(System.Exception exception, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 AddErr(System.Exception exception, string title), uint64 AddErr(string format, Params System.Object[] args), uint64 IXmlLogger.AddErr(System.Exception excSrc, string title, Params System.Object[] args), uint64 IXmlLogger.AddErr(System.Exception excSrc, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddErr(System.Exception excSrc, string title), uint64 IXmlLogger.AddErr(string format, Params System.Object[] args)]
* $VBRBackupSession.Logger.AddLog()  Def [uint64 AddLog(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, Params System.Object[] args), uint64 AddLog(string format, Params System.Object[] args), uint64 AddLog(Veeam.Backup.Common.CTaskLogRecord logRecord), uint64 IXmlLogger.AddLog(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, Params System.Object[] args), uint64 IXmlLogger.AddLog(string format, Params System.Object[] args), uint64 IXmlLogger.AddLog(Veeam.Backup.Common.CTaskLogRecord logRecord)]
* $VBRBackupSession.Logger.AddLogWithDescription()  Def [uint64 AddLogWithDescription(datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility), uint64 AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, Veeam.Backup.Common.ETaskLogStyle style, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility), uint64 IXmlLogger.AddLogWithDescription(datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility), uint64 IXmlLogger.AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, Veeam.Backup.Common.ETaskLogStyle style, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility)]
* $VBRBackupSession.Logger.AddOrUpdateLog()  Def [void AddOrUpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord), void IXmlLogger.AddOrUpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord)]
* $VBRBackupSession.Logger.AddSuccess()  Def [uint64 AddSuccess(string title, Params System.Object[] args), uint64 AddSuccess(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 AddSuccess(string title), uint64 IXmlLogger.AddSuccess(string title, Params System.Object[] args), uint64 IXmlLogger.AddSuccess(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddSuccess(string title)]
* $VBRBackupSession.Logger.AddWarning()  Def [uint64 AddWarning(string title, Params System.Object[] args), uint64 AddWarning(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 AddWarning(System.Exception exception, string title, Params System.Object[] args), uint64 AddWarning(System.Exception exception, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(System.Exception ex, string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(System.Exception ex, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args)]
* $VBRBackupSession.Logger.AddWarningWithDescription()  Def [uint64 AddWarningWithDescription(System.Exception exception, string title, string desc), uint64 IXmlLogger.AddWarningWithDescription(System.Exception ex, string title, string desc)]
* $VBRBackupSession.Logger.ChangeStatus()  Def [void ChangeStatus(Veeam.Backup.Common.ETaskLogRecordStatus fromStatus, Veeam.Backup.Common.ETaskLogRecordStatus toStatus), void IXmlLogger.ChangeStatus(Veeam.Backup.Common.ETaskLogRecordStatus fromStatus, Veeam.Backup.Common.ETaskLogRecordStatus toStatus)]
* $VBRBackupSession.Logger.Clear()  Def [void Clear(), void IXmlLogger.Clear()]
* $VBRBackupSession.Logger.Complete()  Def [void Complete(string[] cookies, Veeam.Backup.Common.ETaskLogRecordStatus status), void Complete(string[] cookies, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status), void Complete(string[] cookiesArray, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string description), void Complete(string[] cookiesArray, Veeam.Backup.Common.ETaskLogRecordStatus status, string description), void Complete(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status), void Complete(string cookie, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status), void IXmlLogger.Complete(string[] cookies, Veeam.Backup.Common.ETaskLogRecordStatus status), void IXmlLogger.Complete(string[] cookies, Veeam.Backup.Common.ETaskLogRecordStatus status, string description), void IXmlLogger.Complete(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status)]
* $VBRBackupSession.Logger.CompleteAll()  Def [void CompleteAll(Veeam.Backup.Common.ETaskLogRecordStatus status, string description), void IXmlLogger.CompleteAll(Veeam.Backup.Common.ETaskLogRecordStatus status, string description)]
* $VBRBackupSession.Logger.CompleteSuccess()  Def [void CompleteSuccess(string cookie), void CompleteSuccess(string cookie, datetime time), void IXmlLogger.CompleteSuccess(string cookie), void IXmlLogger.CompleteSuccess(string cookie, datetime time)]
* $VBRBackupSession.Logger.GetLog()  Def [Veeam.Backup.Common.CTaskLogUpdates GetLog(uint64 usn), Veeam.Backup.Common.CTaskLogUpdates GetLog(), Veeam.Backup.Common.CTaskLogUpdates IXmlLogger.GetLog(), Veeam.Backup.Common.CTaskLogUpdates IXmlLogger.GetLog(uint64 usn)]
* $VBRBackupSession.Logger.GetMaxSeverity()  Def [Veeam.Backup.Common.ETaskLogRecordStatus GetMaxSeverity(), Veeam.Backup.Common.ETaskLogRecordStatus IXmlLogger.GetMaxSeverity()]
* $VBRBackupSession.Logger.GetRecordIdByCookieOrNull()  Def [System.Nullable[uint64] GetRecordIdByCookieOrNull(string cookie), System.Nullable[uint64] IXmlLogger.GetRecordIdByCookieOrNull(string cookie)]
* $VBRBackupSession.Logger.GetTopUsn()  Def [uint64 GetTopUsn(), uint64 IXmlLogger.GetTopUsn()]
* $VBRBackupSession.Logger.IsRecordExistWithCookie()  Def [bool IsRecordExistWithCookie(string cookie), bool IXmlLogger.IsRecordExistWithCookie(string cookie)]
* $VBRBackupSession.Logger.RemoveRecord()  Def [uint64 RemoveRecord(uint64 logRecordId), uint64 IXmlLogger.RemoveRecord(uint64 logRecordId)]
* $VBRBackupSession.Logger.RemoveRecords()  Def [uint64 RemoveRecords(uint64 firstLogRecordId, uint64 lastLogRecordId), uint64 IXmlLogger.RemoveRecords(uint64 firstLogRecordId, uint64 lastLogRecordId)]
* $VBRBackupSession.Logger.SetErr()  Def [uint64 SetErr(string cookie, System.Exception exception, string title, Params System.Object[] args), uint64 SetErr(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetErr(string cookie, System.Exception ex, string title, Params System.Object[] args), uint64 IXmlLogger.SetErr(string cookie, string title, Params System.Object[] args)]
* $VBRBackupSession.Logger.SetInProgress()  Def [uint64 SetInProgress(string cookie, string title, Params System.Object[] args), uint64 SetInProgress(string cookie, datetime time, string title, Params System.Object[] args), uint64 IXmlLogger.SetInProgress(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetInProgress(string cookie, datetime time, string title, Params System.Object[] args)]
* $VBRBackupSession.Logger.SetSuccess()  Def [uint64 SetSuccess(string cookie, string title, Params System.Object[] args), uint64 SetSuccess(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.SetSuccess(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetSuccess(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args)]
* $VBRBackupSession.Logger.SetWarning()  Def [uint64 SetWarning(string cookie, System.Exception exception, string title, Params System.Object[] args), uint64 SetWarning(string cookie, string title, Params System.Object[] args), uint64 SetWarning(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.SetWarning(string cookie, System.Exception ex, string title, Params System.Object[] args), uint64 IXmlLogger.SetWarning(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetWarning(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args)]
* $VBRBackupSession.Logger.TryGetLog()  Def [bool TryGetLog(uint64 usn, [ref] Veeam.Backup.Common.CTaskLogUpdates updates), bool IXmlLogGetter.TryGetLog(uint64 usn, [ref] Veeam.Backup.Common.CTaskLogUpdates updates)]
* $VBRBackupSession.Logger.UpdateErr()  Def [uint64 UpdateErr(uint64 logRecordId, string title, System.Exception exception), uint64 UpdateErr(uint64 logRecordId, string title), void UpdateErr(uint64 logRecordId), uint64 IXmlLogger.UpdateErr(uint64 logRecordId, string title, System.Exception ex), uint64 IXmlLogger.UpdateErr(uint64 logRecordId, string title), void IXmlLogger.UpdateErr(uint64 logRecordId)]
* $VBRBackupSession.Logger.UpdateLog()  Def [uint64 UpdateLog(uint64 logRecordId, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 UpdateLog(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 UpdateLog(uint64 logRecordId, string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 UpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord), uint64 IXmlLogger.UpdateLog(uint64 logRecordId, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.UpdateLog(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.UpdateLog(uint64 logRecordId, string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.UpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord)]
* $VBRBackupSession.Logger.UpdateStatus()  Def [void UpdateStatus(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status), void IXmlLogger.UpdateStatus(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status)]
* $VBRBackupSession.Logger.UpdateSuccess()  Def [uint64 UpdateSuccess(uint64 logRecordId, string title), uint64 IXmlLogger.UpdateSuccess(uint64 logRecordId, string title)]
* $VBRBackupSession.Logger.UpdateWarning()  Def [uint64 UpdateWarning(uint64 logRecordId, string title), uint64 UpdateWarning(uint64 logRecordId, string title, System.Exception exception), uint64 IXmlLogger.UpdateWarning(uint64 logRecordId, string title), uint64 IXmlLogger.UpdateWarning(uint64 logRecordId, string title, System.Exception ex)]
* $VBRBackupSession.Logger.Formatter \[Veeam.Backup.Core.XmlLoggerFormatter\]
* $VBRBackupSession.Logger.Formatter.FormatErrorNoThrow()  Def [string FormatErrorNoThrow(bool isError, System.Exception exception, string title, Params System.Object[] args), string IXmlLoggerFormatter.FormatErrorNoThrow(bool isError, System.Exception exception, string title, Params System.Object[] args)]
* $VBRBackupSession.Logger.Formatter.FormatNoThrow()  Def [string FormatNoThrow(string title, System.Object[] args), string IXmlLoggerFormatter.FormatNoThrow(string title, Params System.Object[] args)]
* $VBRBackupSession.Logger.MinTimeout \[System.Int32\]
* $VBRBackupSession.Logger.SessionId \[System.Guid\]
* $VBRBackupSession.Logger.Token \[Veeam.Backup.Model.CXmlLogToken\]
* $VBRBackupSession.Logger.Token.FormatterType \[Veeam.Backup.Model.EXmlFormatterType\] \($null\)
* $VBRBackupSession.Logger.Token.IsNullLogToken \[System.Boolean\] \($null\)
* $VBRBackupSession.Logger.Token.SessId \[System.Guid\]
* $VBRBackupSession.LogName \[System.String\]
* $VBRBackupSession.LogsSubFolder \[System.String\]
* $VBRBackupSession.MasterKey \[$null\] \($null\)
* $VBRBackupSession.Name \[System.String\]
* $VBRBackupSession.Operation \[System.String\] \($null\)
* $VBRBackupSession.OriginalSessionId \[System.Guid\]
* $VBRBackupSession.OrigJobName \[System.String\]
* $VBRBackupSession.ParentSessionId \[System.Guid\]
* $VBRBackupSession.PostActivity \[Veeam.Backup.Core.CBackupSession+EPostActivity\] \($null\)
* $VBRBackupSession.Progress \[Veeam.Backup.Model.CBackupProgressData\]
* $VBRBackupSession.Progress.AddChildAndGet()  Def [Veeam.Backup.Model.CBackupProgressData AddChildAndGet(System.Object key, Veeam.Backup.Model.CBackupProgressData child)]
* $VBRBackupSession.Progress.ApplyUpdates()  Def [void ApplyUpdates(Veeam.Backup.Model.CBackupProgressUpdates updates)]
* $VBRBackupSession.Progress.CalcAvgSpeed()  Def [void CalcAvgSpeed()]
* $VBRBackupSession.Progress.CalcPercents()  Def [void CalcPercents()]
* $VBRBackupSession.Progress.Clone()  Def [Veeam.Backup.Model.CBackupProgressData Clone()]
* $VBRBackupSession.Progress.ConvertForeignTimeToLocal()  Def [void ConvertForeignTimeToLocal(timespan timeShift)]
* $VBRBackupSession.Progress.DecrementProcessedSize()  Def [void DecrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSession.Progress.DecrementTotalObjects()  Def [void DecrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSession.Progress.DecrementTotalSize()  Def [void DecrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSession.Progress.FindChild()  Def [Veeam.Backup.Model.CBackupProgressData FindChild(System.Object key)]
* $VBRBackupSession.Progress.GetProcessingDuration()  Def [timespan GetProcessingDuration()]
* $VBRBackupSession.Progress.GetRemainingTime()  Def [timespan GetRemainingTime(System.Nullable[long] avgSpeed)]
* $VBRBackupSession.Progress.IncrementProcessedObjects()  Def [void IncrementProcessedObjects(int deltaProcessedObjects)]
* $VBRBackupSession.Progress.IncrementProcessedSize()  Def [void IncrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSession.Progress.IncrementTotalObjects()  Def [void IncrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSession.Progress.IncrementTotalObjectsWithProcessed()  Def [void IncrementTotalObjectsWithProcessed(int newObjects)]
* $VBRBackupSession.Progress.IncrementTotalSize()  Def [void IncrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSession.Progress.IncrementTotalSizeWithProcessed()  Def [void IncrementTotalSizeWithProcessed(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSession.Progress.RemoveChild()  Def [void RemoveChild(System.Object key)]
* $VBRBackupSession.Progress.Serialize()  Def [string Serialize()]
* $VBRBackupSession.Progress.Start()  Def [void Start()]
* $VBRBackupSession.Progress.Stop()  Def [void Stop(System.Nullable[datetime] stopTime)]
* $VBRBackupSession.Progress.UpdateBottleneck()  Def [void UpdateBottleneck(Veeam.Backup.Model.CBottleneckInfo bottleneckInfo)]
* $VBRBackupSession.Progress.UpdateParentTotalSize()  Def [void UpdateParentTotalSize()]
* $VBRBackupSession.Progress.UpdateParentTotalSizeIfZero()  Def [void UpdateParentTotalSizeIfZero()]
* $VBRBackupSession.Progress.UpdateProcessedObjects()  Def [void UpdateProcessedObjects(int processedObjects)]
* $VBRBackupSession.Progress.UpdateProcessedSize()  Def [void UpdateProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSession.Progress.UpdateTime()  Def [void UpdateTime(datetime startTime, datetime stopTime)]
* $VBRBackupSession.Progress.UpdateTotalObjects()  Def [void UpdateTotalObjects(int totalObjects)]
* $VBRBackupSession.Progress.UpdateTotalSize()  Def [void UpdateTotalSize(long totalSize, long totalUsedSize)]
* $VBRBackupSession.Progress.AvgSpeed \[System.Int64\]
* $VBRBackupSession.Progress.BottleneckInfo \[Veeam.Backup.Model.CBottleneckInfo\]
* $VBRBackupSession.Progress.BottleneckInfo.CalcBottleneck()  Def [Veeam.Backup.Model.EBottleneck CalcBottleneck(bool networkThrottlingEnabled, bool targetRepositoryThrottlingEnabled, bool sourceRepositoryThrottlingEnabled)]
* $VBRBackupSession.Progress.BottleneckInfo.GetSettedValues()  Def [System.Tuple[string,int][] GetSettedValues()]
* $VBRBackupSession.Progress.BottleneckInfo.Serial()  Def [void Serial(System.Xml.XmlNode rootNode)]
* $VBRBackupSession.Progress.BottleneckInfo.Update()  Def [void Update(Veeam.Backup.Model.CBottleneckInfo other)]
* $VBRBackupSession.Progress.BottleneckInfo.Bottleneck \[Veeam.Backup.Model.EBottleneck\]
* $VBRBackupSession.Progress.BottleneckInfo.Bottleneck.value__ \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.Network \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.NetworkThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSession.Progress.BottleneckInfo.Proxy \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.RepositoryThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSession.Progress.BottleneckInfo.Source \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.SourceNetwork \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.SourceProxy \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.SourceStorage \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.SourceWan \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.Target \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.TargetNetwork \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.TargetProxy \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.TargetStorage \[System.Int32\]
* $VBRBackupSession.Progress.BottleneckInfo.TargetWan \[System.Int32\]
* $VBRBackupSession.Progress.Duration \[System.TimeSpan\]
* $VBRBackupSession.Progress.IsNeedSubstractReadDelay \[System.Boolean\] \($null\)
* $VBRBackupSession.Progress.Percents \[System.Int32\]
* $VBRBackupSession.Progress.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.ProcessedObjects \[System.Int32\]
* $VBRBackupSession.Progress.ProcessedSize \[System.Int64\]
* $VBRBackupSession.Progress.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.ProcessedUsedSize \[System.Int64\]
* $VBRBackupSession.Progress.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.ReadedAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.ReadedAverageSize \[System.Int64\]
* $VBRBackupSession.Progress.ReadSize \[System.Int64\]
* $VBRBackupSession.Progress.StartTimeLocal \[System.DateTime\]
* $VBRBackupSession.Progress.StartTimeUtc \[System.DateTime\]
* $VBRBackupSession.Progress.StopTimeLocal \[System.DateTime\]
* $VBRBackupSession.Progress.StopTimeUtc \[System.DateTime\]
* $VBRBackupSession.Progress.TotalObjects \[System.Int32\]
* $VBRBackupSession.Progress.TotalSize \[System.Int64\]
* $VBRBackupSession.Progress.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.TotalUsedSize \[System.Int64\]
* $VBRBackupSession.Progress.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.TransferedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.TransferedSize \[System.Int64\]
* $VBRBackupSession.Progress.Updates \[Veeam.Backup.Model.CBackupProgressUpdates\]
* $VBRBackupSession.Progress.Updates.IncrementProcessedDeltas()  Def [void IncrementProcessedDeltas(long processedDeltaIncrement, long processedUsedDeltaIncrement, long readDeltaIncrement, long readAverageDeltaIncrement, long transferredDeltaIncrement)]
* $VBRBackupSession.Progress.Updates.IncrementTotalSizeDeltas()  Def [void IncrementTotalSizeDeltas(long totalSizeDeltaIncrement, long totalUsedSizeDeltaIncrement)]
* $VBRBackupSession.Progress.Updates.Reset()  Def [void Reset()]
* $VBRBackupSession.Progress.Updates.SetChildBottlenecks()  Def [void SetChildBottlenecks(System.Collections.Generic.IDictionary[string,Veeam.Backup.Model.CBottleneckInfo] childBottlenecks)]
* $VBRBackupSession.Progress.Updates.SetChildProcessingIntervals()  Def [void SetChildProcessingIntervals(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Common.CDateTimeInterval][] childIntervals)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks \[System.Collections.Concurrent.ConcurrentDictionary`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.Add()  Def [void IDictionary[string,CBottleneckInfo].Add(string key, Veeam.Backup.Model.CBottleneckInfo value), void ICollection[KeyValuePair[string,CBottleneckInfo]].Add(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Add(System.Object key, System.Object value)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.AddOrUpdate()  Def [Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, Veeam.Backup.Model.CBottleneckInfo addValue, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,TArg,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory, TArg factoryArgument)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.Clear()  Def [void Clear(), void ICollection[KeyValuePair[string,CBottleneckInfo]].Clear(), void IDictionary.Clear()]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.Contains()  Def [bool ICollection[KeyValuePair[string,CBottleneckInfo]].Contains(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), bool IDictionary.Contains(System.Object key)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.ContainsKey()  Def [bool ContainsKey(string key), bool IDictionary[string,CBottleneckInfo].ContainsKey(string key), bool IReadOnlyDictionary[string,CBottleneckInfo].ContainsKey(string key)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.CopyTo()  Def [void ICollection[KeyValuePair[string,CBottleneckInfo]].CopyTo(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo][] array, int arrayIndex), void ICollection.CopyTo(array array, int index)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.GetEnumerator()  Def [System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] GetEnumerator(), System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] IEnumerable[KeyValuePair[string,CBottleneckInfo]].GetEnumerator(), System.Collections.IEnumerator IEnumerable.GetEnumerator(), System.Collections.IDictionaryEnumerator IDictionary.GetEnumerator()]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.GetOrAdd()  Def [Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] valueFactory), Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, Veeam.Backup.Model.CBottleneckInfo value), Veeam.Backup.Model.CBottleneckInfo GetOrAdd[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] valueFactory, TArg factoryArgument)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.Remove()  Def [bool IDictionary[string,CBottleneckInfo].Remove(string key), bool ICollection[KeyValuePair[string,CBottleneckInfo]].Remove(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Remove(System.Object key)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.TryAdd()  Def [bool TryAdd(string key, Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.TryGetValue()  Def [bool TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IReadOnlyDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.TryRemove()  Def [bool TryRemove(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.TryUpdate()  Def [bool TryUpdate(string key, Veeam.Backup.Model.CBottleneckInfo newValue, Veeam.Backup.Model.CBottleneckInfo comparisonValue)]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.Count \[System.Int32\] \($null\)
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.IsEmpty \[System.Boolean\]
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.IsFixedSize \[System.Boolean\] \($null\)
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.IsReadOnly \[System.Boolean\] \($null\)
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.IsSynchronized \[System.Boolean\] \($null\)
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.Keys \[System.Collections.ObjectModel.ReadOnlyCollection`1[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.SyncRoot \[$null\] \($null\)
* $VBRBackupSession.Progress.Updates.ChildBottlenecks.Values \[System.Collections.ObjectModel.ReadOnlyCollection`1[[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\] \($null\)
* $VBRBackupSession.Progress.Updates.ChildProcessingIntervals \[System.Collections.Generic.KeyValuePair`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Common.CDateTimeInterval, Veeam.Backup.Common, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]][]\] \($null\)
* $VBRBackupSession.Progress.Updates.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.Updates.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.Updates.ReadAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.Updates.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.Updates.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.Updates.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.Updates.TransferredDelta \[System.Int64\] \($null\)
* $VBRBackupSession.Progress.UsedSpaceRation \[System.Double\]
* $VBRBackupSession.Result \[Veeam.Backup.Model.CBaseSessionInfo+EResult\] \($null\)
* $VBRBackupSession.SelectiveProcessingSpec \[$null\] \($null\)
* $VBRBackupSession.SessionCryptoSpec \[Veeam.Backup.Crypto.CCryptoSymmetricSpec\]
* $VBRBackupSession.SessionCryptoSpec.CloneWithouKeys()  Def [Veeam.Backup.Crypto.CCryptoSymmetricSpec CloneWithouKeys()]
* $VBRBackupSession.SessionCryptoSpec.CloneWithoutKeys()  Def [Veeam.Backup.Crypto.ICryptoSpec ICryptoSpec.CloneWithoutKeys()]
* $VBRBackupSession.SessionCryptoSpec.CloneWithoutRepair()  Def [Veeam.Backup.Crypto.CCryptoSymmetricSpec CloneWithoutRepair()]
* $VBRBackupSession.SessionCryptoSpec.CreateRecoveryRecord()  Def [void CreateRecoveryRecord(Veeam.Backup.Crypto.CCryptoSymmetricSpec child), void ICryptoSpec.CreateRecoveryRecord(Veeam.Backup.Crypto.CCryptoSymmetricSpec child)]
* $VBRBackupSession.SessionCryptoSpec.Decrypt()  Def [byte[] Decrypt(byte[] bytes)]
* $VBRBackupSession.SessionCryptoSpec.DecryptString()  Def [string DecryptString(string str)]
* $VBRBackupSession.SessionCryptoSpec.Dispose()  Def [void Dispose(), void IDisposable.Dispose()]
* $VBRBackupSession.SessionCryptoSpec.Encrypt()  Def [byte[] Encrypt(byte[] bytes)]
* $VBRBackupSession.SessionCryptoSpec.EncryptString()  Def [string EncryptString(string str)]
* $VBRBackupSession.SessionCryptoSpec.RecoverKeys()  Def [void RecoverKeys(Veeam.Backup.Crypto.CCryptoSymmetricSpec child)]
* $VBRBackupSession.SessionCryptoSpec.CreationTime \[System.DateTime\]
* $VBRBackupSession.SessionCryptoSpec.CryptoAlg \[Veeam.Backup.Crypto.ECryptoAlg\]
* $VBRBackupSession.SessionCryptoSpec.CryptoAlg.value__ \[System.Int32\]
* $VBRBackupSession.SessionCryptoSpec.Hint \[System.String\]
* $VBRBackupSession.SessionCryptoSpec.Id \[Veeam.Backup.Model.CKeySetId\]
* $VBRBackupSession.SessionCryptoSpec.Id.IsEqual()  Def [bool IsEqual(Veeam.Backup.Model.CKeySetId keySetId)]
* $VBRBackupSession.SessionCryptoSpec.Id.IsEmpty \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionCryptoSpec.Id.Value \[System.Byte[]\]
* $VBRBackupSession.SessionCryptoSpec.KeyValue \[Veeam.Backup.Model.CKeyBlob\]
* $VBRBackupSession.SessionCryptoSpec.KeyValue.Dispose()  Def [void Dispose(), void IDisposable.Dispose()]
* $VBRBackupSession.SessionCryptoSpec.KeyValue.IsNullOrEmpty()  Def [bool IsNullOrEmpty()]
* $VBRBackupSession.SessionCryptoSpec.KeyValue.Raw \[System.Byte[]\]
* $VBRBackupSession.SessionCryptoSpec.Raw \[Veeam.Backup.Model.CSerializedKeySet\]
* $VBRBackupSession.SessionCryptoSpec.Raw.AsBase64()  Def [string AsBase64()]
* $VBRBackupSession.SessionCryptoSpec.Raw.Serialize()  Def [string Serialize(), void Serialize(System.Xml.XmlNode node)]
* $VBRBackupSession.SessionCryptoSpec.Raw.IsEmpty \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionCryptoSpec.Raw.Raw \[System.Byte[]\]
* $VBRBackupSession.SessionCryptoSpec.RepairRecs \[Veeam.Backup.Model.CRepairRec[]\] \($null\)
* $VBRBackupSession.SessionCryptoSpec.UsageRole \[Veeam.Backup.Crypto.ECryptoUsageRole\]
* $VBRBackupSession.SessionCryptoSpec.UsageRole.value__ \[System.Int32\]
* $VBRBackupSession.SessionInfo \[Veeam.Backup.Model.CBackupSessionInfo\]
* $VBRBackupSession.SessionInfo.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRBackupSession.SessionInfo.SetJobAlgorithm()  Def [void SetJobAlgorithm(Veeam.Backup.Model.JobAlgorithms algorithm)]
* $VBRBackupSession.SessionInfo.SetSessionAlgorithm()  Def [void SetSessionAlgorithm(Veeam.Backup.Model.SessionAlgorithms algorithm)]
* $VBRBackupSession.SessionInfo.AuxData \[System.String\]
* $VBRBackupSession.SessionInfo.BackedUpSize \[System.Int64\]
* $VBRBackupSession.SessionInfo.BackupTotalSize \[System.Int64\]
* $VBRBackupSession.SessionInfo.CompletionPercentage \[System.Int32\]
* $VBRBackupSession.SessionInfo.CreationTime \[System.DateTime\]
* $VBRBackupSession.SessionInfo.CurrentPointId \[System.Guid\]
* $VBRBackupSession.SessionInfo.Description \[System.String\] \($null\)
* $VBRBackupSession.SessionInfo.EndTime \[System.DateTime\]
* $VBRBackupSession.SessionInfo.Failures \[System.Int32\] \($null\)
* $VBRBackupSession.SessionInfo.Id \[System.Guid\]
* $VBRBackupSession.SessionInfo.Initiator \[Veeam.Backup.Model.CBaseSessionInfo+SInitiator\]
* $VBRBackupSession.SessionInfo.Initiator.Name \[$null\] \($null\)
* $VBRBackupSession.SessionInfo.Initiator.Sid \[$null\] \($null\)
* $VBRBackupSession.SessionInfo.Initiator2 \[Veeam.Backup.Model.CModifiedUserInfo\]
* $VBRBackupSession.SessionInfo.Initiator2.Serialize()  Def [string Serialize(), void Serialize(System.Xml.XmlNode node)]
* $VBRBackupSession.SessionInfo.Initiator2.FullName \[System.String\] \($null\)
* $VBRBackupSession.SessionInfo.Initiator2.LoginType \[Veeam.Backup.Model.EModifiedUserType\]
* $VBRBackupSession.SessionInfo.Initiator2.LoginType.value__ \[System.Int32\]
* $VBRBackupSession.SessionInfo.IsActiveFullMode \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.IsCompleted \[System.Boolean\]
* $VBRBackupSession.SessionInfo.IsFullMode \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.IsRecheckRetry \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.IsRetryMode \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.IsWorking \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.JobAlgorithm \[Veeam.Backup.Model.JobAlgorithms\]
* $VBRBackupSession.SessionInfo.JobAlgorithm.value__ \[System.Int32\]
* $VBRBackupSession.SessionInfo.JobId \[System.Guid\]
* $VBRBackupSession.SessionInfo.JobName \[System.String\]
* $VBRBackupSession.SessionInfo.JobSourceType \[Veeam.Backup.Model.CDbBackupJobInfo+ESourceType\]
* $VBRBackupSession.SessionInfo.JobSourceType.value__ \[System.Int32\]
* $VBRBackupSession.SessionInfo.JobSpec \[System.String\] \($null\)
* $VBRBackupSession.SessionInfo.JobType \[Veeam.Backup.Model.EDbJobType\] \($null\)
* $VBRBackupSession.SessionInfo.LeaseId \[System.Guid\]
* $VBRBackupSession.SessionInfo.LogsSubFolder \[System.String\]
* $VBRBackupSession.SessionInfo.Operation \[System.String\] \($null\)
* $VBRBackupSession.SessionInfo.OriginalSessionId \[System.Guid\]
* $VBRBackupSession.SessionInfo.ParentSessionId \[System.Guid\]
* $VBRBackupSession.SessionInfo.Platform \[Veeam.Backup.Common.CPlatform\]
* $VBRBackupSession.SessionInfo.Platform.IsExternalInfrastructure()  Def [bool IsExternalInfrastructure()]
* $VBRBackupSession.SessionInfo.Platform.IsWellKnown()  Def [bool IsWellKnown()]
* $VBRBackupSession.SessionInfo.Platform.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRBackupSession.SessionInfo.Platform.Platform \[Veeam.Backup.Common.EPlatform\] \($null\)
* $VBRBackupSession.SessionInfo.Platform.PlatformId \[System.Guid\]
* $VBRBackupSession.SessionInfo.PolicyName \[System.String\] \($null\)
* $VBRBackupSession.SessionInfo.PolicyTag \[System.String\] \($null\)
* $VBRBackupSession.SessionInfo.Progress \[Veeam.Backup.Model.CBackupProgressData\]
* $VBRBackupSession.SessionInfo.Progress.AddChildAndGet()  Def [Veeam.Backup.Model.CBackupProgressData AddChildAndGet(System.Object key, Veeam.Backup.Model.CBackupProgressData child)]
* $VBRBackupSession.SessionInfo.Progress.ApplyUpdates()  Def [void ApplyUpdates(Veeam.Backup.Model.CBackupProgressUpdates updates)]
* $VBRBackupSession.SessionInfo.Progress.CalcAvgSpeed()  Def [void CalcAvgSpeed()]
* $VBRBackupSession.SessionInfo.Progress.CalcPercents()  Def [void CalcPercents()]
* $VBRBackupSession.SessionInfo.Progress.Clone()  Def [Veeam.Backup.Model.CBackupProgressData Clone()]
* $VBRBackupSession.SessionInfo.Progress.ConvertForeignTimeToLocal()  Def [void ConvertForeignTimeToLocal(timespan timeShift)]
* $VBRBackupSession.SessionInfo.Progress.DecrementProcessedSize()  Def [void DecrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSession.SessionInfo.Progress.DecrementTotalObjects()  Def [void DecrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSession.SessionInfo.Progress.DecrementTotalSize()  Def [void DecrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSession.SessionInfo.Progress.FindChild()  Def [Veeam.Backup.Model.CBackupProgressData FindChild(System.Object key)]
* $VBRBackupSession.SessionInfo.Progress.GetProcessingDuration()  Def [timespan GetProcessingDuration()]
* $VBRBackupSession.SessionInfo.Progress.GetRemainingTime()  Def [timespan GetRemainingTime(System.Nullable[long] avgSpeed)]
* $VBRBackupSession.SessionInfo.Progress.IncrementProcessedObjects()  Def [void IncrementProcessedObjects(int deltaProcessedObjects)]
* $VBRBackupSession.SessionInfo.Progress.IncrementProcessedSize()  Def [void IncrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSession.SessionInfo.Progress.IncrementTotalObjects()  Def [void IncrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSession.SessionInfo.Progress.IncrementTotalObjectsWithProcessed()  Def [void IncrementTotalObjectsWithProcessed(int newObjects)]
* $VBRBackupSession.SessionInfo.Progress.IncrementTotalSize()  Def [void IncrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSession.SessionInfo.Progress.IncrementTotalSizeWithProcessed()  Def [void IncrementTotalSizeWithProcessed(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSession.SessionInfo.Progress.RemoveChild()  Def [void RemoveChild(System.Object key)]
* $VBRBackupSession.SessionInfo.Progress.Serialize()  Def [string Serialize()]
* $VBRBackupSession.SessionInfo.Progress.Start()  Def [void Start()]
* $VBRBackupSession.SessionInfo.Progress.Stop()  Def [void Stop(System.Nullable[datetime] stopTime)]
* $VBRBackupSession.SessionInfo.Progress.UpdateBottleneck()  Def [void UpdateBottleneck(Veeam.Backup.Model.CBottleneckInfo bottleneckInfo)]
* $VBRBackupSession.SessionInfo.Progress.UpdateParentTotalSize()  Def [void UpdateParentTotalSize()]
* $VBRBackupSession.SessionInfo.Progress.UpdateParentTotalSizeIfZero()  Def [void UpdateParentTotalSizeIfZero()]
* $VBRBackupSession.SessionInfo.Progress.UpdateProcessedObjects()  Def [void UpdateProcessedObjects(int processedObjects)]
* $VBRBackupSession.SessionInfo.Progress.UpdateProcessedSize()  Def [void UpdateProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSession.SessionInfo.Progress.UpdateTime()  Def [void UpdateTime(datetime startTime, datetime stopTime)]
* $VBRBackupSession.SessionInfo.Progress.UpdateTotalObjects()  Def [void UpdateTotalObjects(int totalObjects)]
* $VBRBackupSession.SessionInfo.Progress.UpdateTotalSize()  Def [void UpdateTotalSize(long totalSize, long totalUsedSize)]
* $VBRBackupSession.SessionInfo.Progress.AvgSpeed \[System.Int64\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo \[Veeam.Backup.Model.CBottleneckInfo\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.CalcBottleneck()  Def [Veeam.Backup.Model.EBottleneck CalcBottleneck(bool networkThrottlingEnabled, bool targetRepositoryThrottlingEnabled, bool sourceRepositoryThrottlingEnabled)]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.GetSettedValues()  Def [System.Tuple[string,int][] GetSettedValues()]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.Serial()  Def [void Serial(System.Xml.XmlNode rootNode)]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.Update()  Def [void Update(Veeam.Backup.Model.CBottleneckInfo other)]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.Bottleneck \[Veeam.Backup.Model.EBottleneck\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.Bottleneck.value__ \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.Network \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.NetworkThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.Proxy \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.RepositoryThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.Source \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.SourceNetwork \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.SourceProxy \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.SourceStorage \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.SourceWan \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.Target \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.TargetNetwork \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.TargetProxy \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.TargetStorage \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.BottleneckInfo.TargetWan \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.Duration \[System.TimeSpan\]
* $VBRBackupSession.SessionInfo.Progress.IsNeedSubstractReadDelay \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Percents \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.ProcessedObjects \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.ProcessedSize \[System.Int64\]
* $VBRBackupSession.SessionInfo.Progress.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.ProcessedUsedSize \[System.Int64\]
* $VBRBackupSession.SessionInfo.Progress.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.ReadedAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.ReadedAverageSize \[System.Int64\]
* $VBRBackupSession.SessionInfo.Progress.ReadSize \[System.Int64\]
* $VBRBackupSession.SessionInfo.Progress.StartTimeLocal \[System.DateTime\]
* $VBRBackupSession.SessionInfo.Progress.StartTimeUtc \[System.DateTime\]
* $VBRBackupSession.SessionInfo.Progress.StopTimeLocal \[System.DateTime\]
* $VBRBackupSession.SessionInfo.Progress.StopTimeUtc \[System.DateTime\]
* $VBRBackupSession.SessionInfo.Progress.TotalObjects \[System.Int32\]
* $VBRBackupSession.SessionInfo.Progress.TotalSize \[System.Int64\]
* $VBRBackupSession.SessionInfo.Progress.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.TotalUsedSize \[System.Int64\]
* $VBRBackupSession.SessionInfo.Progress.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.TransferedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.TransferedSize \[System.Int64\]
* $VBRBackupSession.SessionInfo.Progress.Updates \[Veeam.Backup.Model.CBackupProgressUpdates\]
* $VBRBackupSession.SessionInfo.Progress.Updates.IncrementProcessedDeltas()  Def [void IncrementProcessedDeltas(long processedDeltaIncrement, long processedUsedDeltaIncrement, long readDeltaIncrement, long readAverageDeltaIncrement, long transferredDeltaIncrement)]
* $VBRBackupSession.SessionInfo.Progress.Updates.IncrementTotalSizeDeltas()  Def [void IncrementTotalSizeDeltas(long totalSizeDeltaIncrement, long totalUsedSizeDeltaIncrement)]
* $VBRBackupSession.SessionInfo.Progress.Updates.Reset()  Def [void Reset()]
* $VBRBackupSession.SessionInfo.Progress.Updates.SetChildBottlenecks()  Def [void SetChildBottlenecks(System.Collections.Generic.IDictionary[string,Veeam.Backup.Model.CBottleneckInfo] childBottlenecks)]
* $VBRBackupSession.SessionInfo.Progress.Updates.SetChildProcessingIntervals()  Def [void SetChildProcessingIntervals(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Common.CDateTimeInterval][] childIntervals)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks \[System.Collections.Concurrent.ConcurrentDictionary`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.Add()  Def [void IDictionary[string,CBottleneckInfo].Add(string key, Veeam.Backup.Model.CBottleneckInfo value), void ICollection[KeyValuePair[string,CBottleneckInfo]].Add(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Add(System.Object key, System.Object value)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.AddOrUpdate()  Def [Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, Veeam.Backup.Model.CBottleneckInfo addValue, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,TArg,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory, TArg factoryArgument)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.Clear()  Def [void Clear(), void ICollection[KeyValuePair[string,CBottleneckInfo]].Clear(), void IDictionary.Clear()]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.Contains()  Def [bool ICollection[KeyValuePair[string,CBottleneckInfo]].Contains(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), bool IDictionary.Contains(System.Object key)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.ContainsKey()  Def [bool ContainsKey(string key), bool IDictionary[string,CBottleneckInfo].ContainsKey(string key), bool IReadOnlyDictionary[string,CBottleneckInfo].ContainsKey(string key)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.CopyTo()  Def [void ICollection[KeyValuePair[string,CBottleneckInfo]].CopyTo(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo][] array, int arrayIndex), void ICollection.CopyTo(array array, int index)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.GetEnumerator()  Def [System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] GetEnumerator(), System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] IEnumerable[KeyValuePair[string,CBottleneckInfo]].GetEnumerator(), System.Collections.IEnumerator IEnumerable.GetEnumerator(), System.Collections.IDictionaryEnumerator IDictionary.GetEnumerator()]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.GetOrAdd()  Def [Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] valueFactory), Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, Veeam.Backup.Model.CBottleneckInfo value), Veeam.Backup.Model.CBottleneckInfo GetOrAdd[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] valueFactory, TArg factoryArgument)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.Remove()  Def [bool IDictionary[string,CBottleneckInfo].Remove(string key), bool ICollection[KeyValuePair[string,CBottleneckInfo]].Remove(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Remove(System.Object key)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.TryAdd()  Def [bool TryAdd(string key, Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.TryGetValue()  Def [bool TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IReadOnlyDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.TryRemove()  Def [bool TryRemove(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.TryUpdate()  Def [bool TryUpdate(string key, Veeam.Backup.Model.CBottleneckInfo newValue, Veeam.Backup.Model.CBottleneckInfo comparisonValue)]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.Count \[System.Int32\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.IsEmpty \[System.Boolean\]
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.IsFixedSize \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.IsReadOnly \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.IsSynchronized \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.Keys \[System.Collections.ObjectModel.ReadOnlyCollection`1[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.SyncRoot \[$null\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildBottlenecks.Values \[System.Collections.ObjectModel.ReadOnlyCollection`1[[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.ChildProcessingIntervals \[System.Collections.Generic.KeyValuePair`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Common.CDateTimeInterval, Veeam.Backup.Common, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]][]\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.ReadAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.Updates.TransferredDelta \[System.Int64\] \($null\)
* $VBRBackupSession.SessionInfo.Progress.UsedSpaceRation \[System.Double\]
* $VBRBackupSession.SessionInfo.Result \[Veeam.Backup.Model.CBaseSessionInfo+EResult\] \($null\)
* $VBRBackupSession.SessionInfo.RunManually \[System.Boolean\] \($null\)
* $VBRBackupSession.SessionInfo.SessionAlgorithm \[Veeam.Backup.Model.SessionAlgorithms\]
* $VBRBackupSession.SessionInfo.SessionAlgorithm.value__ \[System.Int32\]
* $VBRBackupSession.SessionInfo.State \[Veeam.Backup.Model.CBaseSessionInfo+EState\]
* $VBRBackupSession.SessionInfo.State.value__ \[System.Int32\]
* $VBRBackupSession.SessionInfo.TransportType \[Veeam.Backup.Model.ETransportType\]
* $VBRBackupSession.SessionInfo.TransportType.value__ \[System.Int32\]
* $VBRBackupSession.SessionInfo.Warnings \[System.Int32\] \($null\)
* $VBRBackupSession.SessionInfo.WillBeRetried \[System.Boolean\] \($null\)
* $VBRBackupSession.SplitStoragesPerVm \[System.Boolean\] \($null\)
* $VBRBackupSession.StartupMode \[Veeam.Backup.Model.CDbBackupJobInfo+Mode\] \($null\)
* $VBRBackupSession.State \[Veeam.Backup.Model.CBaseSessionInfo+EState\]
* $VBRBackupSession.State.value__ \[System.Int32\]
* $VBRBackupSession.Tracer \[Veeam.Backup.Core.CSessionLogTracer\]
* $VBRBackupSession.Tracer.TraceError()  Def [void TraceError(), void TraceError(string formatMsg, Params string[] args)]
* $VBRBackupSession.Tracer.TraceException()  Def [void TraceException(System.Exception excSrc), void ILogTracer.TraceException(System.Exception excSrc)]
* $VBRBackupSession.Tracer.TraceIfDifferentText()  Def [void TraceIfDifferentText(string formatMsg, Params string[] args)]
* $VBRBackupSession.Tracer.TraceNext()  Def [void TraceNext(Veeam.Backup.Common.ELogRecordVisibility visibility, string formatMsg, Params string[] args), void TraceNext(string formatMsg, Params string[] args), void ILogTracer.TraceNext(string formatMsg, Params string[] args), void ILogTracer.TraceNext(Veeam.Backup.Common.ELogRecordVisibility visibility, string formatMsg, Params string[] args)]
* $VBRBackupSession.Tracer.TraceOk()  Def [void TraceOk(), void ILogTracer.TraceOk()]
* $VBRBackupSession.Tracer.TraceWarning()  Def [void TraceWarning(), void TraceWarning(string formatMsg, Params string[] args)]
* $VBRBackupSession.UserCryptoSpec \[$null\] \($null\)
* $VBRBackupSession.UserKey \[$null\] \($null\)
* $VBRBackupSession.WillBeRetried \[System.Boolean\] \($null\)
* $VBRBackupSession.WorkDetails \[Veeam.Backup.Core.CBackupSessionWorkDetails\]
* $VBRBackupSession.WorkDetails.GetRecheckInfo()  Def [Veeam.Backup.Core.CBackupSessionRecheckInfo GetRecheckInfo()]
* $VBRBackupSession.WorkDetails.RecheckInfo \[$null\] \($null\)
* $VBRBackupSession.WorkDetails.WorkDuration \[System.TimeSpan\]



