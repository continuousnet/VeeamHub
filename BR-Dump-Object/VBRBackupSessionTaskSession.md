# VBRBackupSessionTaskSession [Veeam.Backup.Core.CBackupTaskSession]
``` powershell
$VBRBackupSession = @(Get-VBRBackupSession | ? {$_.JobType -eq "Backup"})[0]
$VBRBackupSessionTaskSession = @($VBRBackupSession.GetTaskSessions())[0]
```
* $VBRBackupSessionTaskSession.CalcExpectedStatus()  Def [Veeam.Backup.Model.ESessionStatus CalcExpectedStatus()]
* $VBRBackupSessionTaskSession.Complete()  Def [void Complete(), void Complete(bool isVmTask, bool notByRetry), void ITaskSession.Complete()]
* $VBRBackupSessionTaskSession.CompleteNoThrow()  Def [void CompleteNoThrow()]
* $VBRBackupSessionTaskSession.DisableRetry()  Def [void DisableRetry(), void ITaskSession.DisableRetry()]
* $VBRBackupSessionTaskSession.Fail()  Def [void Fail(System.Exception ex, string format, Params System.Object[] args), void Fail(bool isVmTask, System.Exception ex, string message), void ITaskSession.Fail(System.Exception ex, string foramt, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.FailWithWarning()  Def [void FailWithWarning(System.Exception ex, string format, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.GetChangeTrackingAsString()  Def [string GetChangeTrackingAsString()]
* $VBRBackupSessionTaskSession.GetDetails()  Def [string GetDetails()]
* $VBRBackupSessionTaskSession.GetModeAsString()  Def [string GetModeAsString()]
* $VBRBackupSessionTaskSession.IncrementTrafficBlockCorruptCount()  Def [void IncrementTrafficBlockCorruptCount()]
* $VBRBackupSessionTaskSession.IsCompleted()  Def [bool IsCompleted()]
* $VBRBackupSessionTaskSession.LogProgress()  Def [void LogProgress(Veeam.Backup.AgentProvider.IProgressEventArgsEx args)]
* $VBRBackupSessionTaskSession.LogProgressAndGetDiskNum()  Def [int LogProgressAndGetDiskNum(Veeam.Backup.AgentProvider.IProgressEventArgsEx args)]
* $VBRBackupSessionTaskSession.MarkForExecution()  Def [void MarkForExecution(Veeam.Backup.Core.IBackupTask task), void MarkForExecution(string taskName)]
* $VBRBackupSessionTaskSession.RegisterDisposable()  Def [void RegisterDisposable(System.IDisposable disposable)]
* $VBRBackupSessionTaskSession.ResetTaskEventNotifier()  Def [void ResetTaskEventNotifier()]
* $VBRBackupSessionTaskSession.SetChangeTracking()  Def [void SetChangeTracking(bool changeTracking)]
* $VBRBackupSessionTaskSession.SetFsAwareInfoLoadFailed()  Def [void SetFsAwareInfoLoadFailed()]
* $VBRBackupSessionTaskSession.SetResult()  Def [void SetResult(Veeam.Backup.Model.ESessionStatus status, string desc)]
* $VBRBackupSessionTaskSession.SetStatus()  Def [void SetStatus(Veeam.Backup.Model.ESessionStatus status)]
* $VBRBackupSessionTaskSession.StopJob()  Def [void StopJob()]
* $VBRBackupSessionTaskSession.TraceException()  Def [void TraceException(System.Exception excSrc)]
* $VBRBackupSessionTaskSession.TraceNext()  Def [void TraceNext(string formatMsg, Params string[] args)]
* $VBRBackupSessionTaskSession.TraceOk()  Def [void TraceOk()]
* $VBRBackupSessionTaskSession.Update()  Def [void Update(guid objectId, Veeam.Backup.Model.CBackupTaskSessionInfo+ESourceMode sourceMode)]
* $VBRBackupSessionTaskSession.UpdateDiskProcessStatisticSafe()  Def [void UpdateDiskProcessStatisticSafe(string diskId, Veeam.Backup.AgentProvider.IProgressEventArgsEx arg, Veeam.Backup.Model.ETransportType transportType, bool isTaskCompleted)]
* $VBRBackupSessionTaskSession.UpdateProgressInfo()  Def [void UpdateProgressInfo(Veeam.Backup.AgentProvider.IProgressEventArgsEx args), void UpdateProgressInfo()]
* $VBRBackupSessionTaskSession.UpdateRetryStatus()  Def [void UpdateRetryStatus(bool retryFlag, int retryNumber)]
* $VBRBackupSessionTaskSession.UpdateTaskEventNotifier()  Def [void UpdateTaskEventNotifier(guid objectId)]
* $VBRBackupSessionTaskSession.UpdateWorkDetails()  Def [void UpdateWorkDetails()]
* $VBRBackupSessionTaskSession.VerifyStop()  Def [void VerifyStop(Veeam.Backup.AgentProvider.CProgressEventArgsEx args)]
* $VBRBackupSessionTaskSession.CurrentDiskNum \[System.Int32\]
* $VBRBackupSessionTaskSession.Id \[System.Guid\]
* $VBRBackupSessionTaskSession.Info \[Veeam.Backup.Model.CBackupTaskSessionInfo\]
* $VBRBackupSessionTaskSession.Info.IsStopped()  Def [bool IsStopped()]
* $VBRBackupSessionTaskSession.Info.ChangeTracking \[System.Boolean\]
* $VBRBackupSessionTaskSession.Info.FormattedIpAddress \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.Info.Id \[System.Guid\]
* $VBRBackupSessionTaskSession.Info.ObjectId \[System.Guid\]
* $VBRBackupSessionTaskSession.Info.ObjectName \[System.String\]
* $VBRBackupSessionTaskSession.Info.ObjectPlatform \[Veeam.Backup.Common.EPlatform\] \($null\)
* $VBRBackupSessionTaskSession.Info.Operation \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress \[Veeam.Backup.Model.CBackupProgressData\]
* $VBRBackupSessionTaskSession.Info.Progress.AddChildAndGet()  Def [Veeam.Backup.Model.CBackupProgressData AddChildAndGet(System.Object key, Veeam.Backup.Model.CBackupProgressData child)]
* $VBRBackupSessionTaskSession.Info.Progress.ApplyUpdates()  Def [void ApplyUpdates(Veeam.Backup.Model.CBackupProgressUpdates updates)]
* $VBRBackupSessionTaskSession.Info.Progress.CalcAvgSpeed()  Def [void CalcAvgSpeed()]
* $VBRBackupSessionTaskSession.Info.Progress.CalcPercents()  Def [void CalcPercents()]
* $VBRBackupSessionTaskSession.Info.Progress.Clone()  Def [Veeam.Backup.Model.CBackupProgressData Clone()]
* $VBRBackupSessionTaskSession.Info.Progress.ConvertForeignTimeToLocal()  Def [void ConvertForeignTimeToLocal(timespan timeShift)]
* $VBRBackupSessionTaskSession.Info.Progress.DecrementProcessedSize()  Def [void DecrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.Info.Progress.DecrementTotalObjects()  Def [void DecrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.Info.Progress.DecrementTotalSize()  Def [void DecrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.Info.Progress.FindChild()  Def [Veeam.Backup.Model.CBackupProgressData FindChild(System.Object key)]
* $VBRBackupSessionTaskSession.Info.Progress.GetProcessingDuration()  Def [timespan GetProcessingDuration()]
* $VBRBackupSessionTaskSession.Info.Progress.GetRemainingTime()  Def [timespan GetRemainingTime(System.Nullable[long] avgSpeed)]
* $VBRBackupSessionTaskSession.Info.Progress.IncrementProcessedObjects()  Def [void IncrementProcessedObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.Info.Progress.IncrementProcessedSize()  Def [void IncrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.Info.Progress.IncrementTotalObjects()  Def [void IncrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.Info.Progress.IncrementTotalObjectsWithProcessed()  Def [void IncrementTotalObjectsWithProcessed(int newObjects)]
* $VBRBackupSessionTaskSession.Info.Progress.IncrementTotalSize()  Def [void IncrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.Info.Progress.IncrementTotalSizeWithProcessed()  Def [void IncrementTotalSizeWithProcessed(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.Info.Progress.RemoveChild()  Def [void RemoveChild(System.Object key)]
* $VBRBackupSessionTaskSession.Info.Progress.Serialize()  Def [string Serialize()]
* $VBRBackupSessionTaskSession.Info.Progress.Start()  Def [void Start()]
* $VBRBackupSessionTaskSession.Info.Progress.Stop()  Def [void Stop(System.Nullable[datetime] stopTime)]
* $VBRBackupSessionTaskSession.Info.Progress.UpdateBottleneck()  Def [void UpdateBottleneck(Veeam.Backup.Model.CBottleneckInfo bottleneckInfo)]
* $VBRBackupSessionTaskSession.Info.Progress.UpdateParentTotalSize()  Def [void UpdateParentTotalSize()]
* $VBRBackupSessionTaskSession.Info.Progress.UpdateParentTotalSizeIfZero()  Def [void UpdateParentTotalSizeIfZero()]
* $VBRBackupSessionTaskSession.Info.Progress.UpdateProcessedObjects()  Def [void UpdateProcessedObjects(int processedObjects)]
* $VBRBackupSessionTaskSession.Info.Progress.UpdateProcessedSize()  Def [void UpdateProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.Info.Progress.UpdateTime()  Def [void UpdateTime(datetime startTime, datetime stopTime)]
* $VBRBackupSessionTaskSession.Info.Progress.UpdateTotalObjects()  Def [void UpdateTotalObjects(int totalObjects)]
* $VBRBackupSessionTaskSession.Info.Progress.UpdateTotalSize()  Def [void UpdateTotalSize(long totalSize, long totalUsedSize)]
* $VBRBackupSessionTaskSession.Info.Progress.AvgSpeed \[System.Int64\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo \[Veeam.Backup.Model.CBottleneckInfo\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.CalcBottleneck()  Def [Veeam.Backup.Model.EBottleneck CalcBottleneck(bool networkThrottlingEnabled, bool targetRepositoryThrottlingEnabled, bool sourceRepositoryThrottlingEnabled)]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.GetSettedValues()  Def [System.Tuple[string,int][] GetSettedValues()]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.Serial()  Def [void Serial(System.Xml.XmlNode rootNode)]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.Update()  Def [void Update(Veeam.Backup.Model.CBottleneckInfo other)]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.Bottleneck \[Veeam.Backup.Model.EBottleneck\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.Network \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.NetworkThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.Proxy \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.RepositoryThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.Source \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.SourceNetwork \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.SourceProxy \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.SourceStorage \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.SourceWan \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.Target \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.TargetNetwork \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.TargetProxy \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.TargetStorage \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.BottleneckInfo.TargetWan \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.Duration \[System.TimeSpan\]
* $VBRBackupSessionTaskSession.Info.Progress.IsNeedSubstractReadDelay \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Percents \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.ProcessedObjects \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.ProcessedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Info.Progress.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.ProcessedUsedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Info.Progress.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.ReadedAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.ReadedAverageSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Info.Progress.ReadSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Info.Progress.StartTimeLocal \[System.DateTime\]
* $VBRBackupSessionTaskSession.Info.Progress.StartTimeUtc \[System.DateTime\]
* $VBRBackupSessionTaskSession.Info.Progress.StopTimeLocal \[System.DateTime\]
* $VBRBackupSessionTaskSession.Info.Progress.StopTimeUtc \[System.DateTime\]
* $VBRBackupSessionTaskSession.Info.Progress.TotalObjects \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.Progress.TotalSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Info.Progress.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.TotalUsedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Info.Progress.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.TransferedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.TransferedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Info.Progress.Updates \[Veeam.Backup.Model.CBackupProgressUpdates\]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.IncrementProcessedDeltas()  Def [void IncrementProcessedDeltas(long processedDeltaIncrement, long processedUsedDeltaIncrement, long readDeltaIncrement, long readAverageDeltaIncrement, long transferredDeltaIncrement)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.IncrementTotalSizeDeltas()  Def [void IncrementTotalSizeDeltas(long totalSizeDeltaIncrement, long totalUsedSizeDeltaIncrement)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.Reset()  Def [void Reset()]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.SetChildBottlenecks()  Def [void SetChildBottlenecks(System.Collections.Generic.IDictionary[string,Veeam.Backup.Model.CBottleneckInfo] childBottlenecks)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.SetChildProcessingIntervals()  Def [void SetChildProcessingIntervals(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Common.CDateTimeInterval][] childIntervals)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks \[System.Collections.Concurrent.ConcurrentDictionary`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.Add()  Def [void IDictionary[string,CBottleneckInfo].Add(string key, Veeam.Backup.Model.CBottleneckInfo value), void ICollection[KeyValuePair[string,CBottleneckInfo]].Add(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Add(System.Object key, System.Object value)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.AddOrUpdate()  Def [Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, Veeam.Backup.Model.CBottleneckInfo addValue, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,TArg,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory, TArg factoryArgument)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.Clear()  Def [void Clear(), void ICollection[KeyValuePair[string,CBottleneckInfo]].Clear(), void IDictionary.Clear()]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.Contains()  Def [bool ICollection[KeyValuePair[string,CBottleneckInfo]].Contains(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), bool IDictionary.Contains(System.Object key)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.ContainsKey()  Def [bool ContainsKey(string key), bool IDictionary[string,CBottleneckInfo].ContainsKey(string key), bool IReadOnlyDictionary[string,CBottleneckInfo].ContainsKey(string key)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.CopyTo()  Def [void ICollection[KeyValuePair[string,CBottleneckInfo]].CopyTo(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo][] array, int arrayIndex), void ICollection.CopyTo(array array, int index)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.GetEnumerator()  Def [System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] GetEnumerator(), System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] IEnumerable[KeyValuePair[string,CBottleneckInfo]].GetEnumerator(), System.Collections.IEnumerator IEnumerable.GetEnumerator(), System.Collections.IDictionaryEnumerator IDictionary.GetEnumerator()]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.GetOrAdd()  Def [Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] valueFactory), Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, Veeam.Backup.Model.CBottleneckInfo value), Veeam.Backup.Model.CBottleneckInfo GetOrAdd[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] valueFactory, TArg factoryArgument)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.Remove()  Def [bool IDictionary[string,CBottleneckInfo].Remove(string key), bool ICollection[KeyValuePair[string,CBottleneckInfo]].Remove(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Remove(System.Object key)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.TryAdd()  Def [bool TryAdd(string key, Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.TryGetValue()  Def [bool TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IReadOnlyDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.TryRemove()  Def [bool TryRemove(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.TryUpdate()  Def [bool TryUpdate(string key, Veeam.Backup.Model.CBottleneckInfo newValue, Veeam.Backup.Model.CBottleneckInfo comparisonValue)]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.Count \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.IsEmpty \[System.Boolean\]
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.IsFixedSize \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.IsReadOnly \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.IsSynchronized \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.Keys \[System.Collections.ObjectModel.ReadOnlyCollection`1[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.SyncRoot \[$null\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildBottlenecks.Values \[System.Collections.ObjectModel.ReadOnlyCollection`1[[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ChildProcessingIntervals \[System.Collections.Generic.KeyValuePair`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Common.CDateTimeInterval, Veeam.Backup.Common, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]][]\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ReadAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.Updates.TransferredDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Info.Progress.UsedSpaceRation \[System.Double\]
* $VBRBackupSessionTaskSession.Info.QueuedTime \[System.DateTime\]
* $VBRBackupSessionTaskSession.Info.Reason \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.Info.RetryCounter \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.Info.SessionId \[System.Guid\]
* $VBRBackupSessionTaskSession.Info.SourceMode \[Veeam.Backup.Model.CBackupTaskSessionInfo+ESourceMode\] \($null\)
* $VBRBackupSessionTaskSession.Info.Status \[Veeam.Backup.Model.ESessionStatus\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails \[Veeam.Backup.Model.CBackupTaskWorkDetails\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.AddCreatedOib()  Def [void AddCreatedOib(guid id)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.GetCreatedOibs()  Def [guid[] GetCreatedOibs()]
* $VBRBackupSessionTaskSession.Info.WorkDetails.RemoveCreatedOib()  Def [void RemoveCreatedOib(guid id)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.Serial()  Def [string Serial()]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetCannotUseCBT()  Def [void SetCannotUseCBT(string reason)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetEpDiscoveryDetails()  Def [void SetEpDiscoveryDetails(Veeam.Backup.Model.Sources.Sessions.CEpDiscoverySessionDetails details)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetEpPolicyDetails()  Def [void SetEpPolicyDetails(bool configurationSent)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetHvDatastoreUsages()  Def [void SetHvDatastoreUsages(Veeam.Backup.Model.CHvDatastoreUsage[] hvDatastoreUsages)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetNoRetry()  Def [void SetNoRetry(bool value)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetOibInfo()  Def [void SetOibInfo(guid oibId)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetRepositoryInfo()  Def [void SetRepositoryInfo(guid repositoryId)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetSourceProxyInfo()  Def [void SetSourceProxyInfo(guid proxyId, int transportMode)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetSourceReportedFailoverToNbd()  Def [void SetSourceReportedFailoverToNbd()]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetSourceRepositoryInfo()  Def [void SetSourceRepositoryInfo(guid repositoryId)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetTargetProxyInfo()  Def [void SetTargetProxyInfo(guid proxyId, int transportMode)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetTargetReportedFailoverToNbd()  Def [void SetTargetReportedFailoverToNbd()]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetTaskAlgorithm()  Def [void SetTaskAlgorithm(Veeam.Backup.Model.ETaskAlgorithm algorithm)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetViDatastoreUsages()  Def [void SetViDatastoreUsages(Veeam.Backup.Model.CViDatastoreUsage[] viDatastoreUsages)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SetWorkDuration()  Def [void SetWorkDuration(timespan workDuration)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.CannotUseCBT \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.CannotUseCBTReason \[$null\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.ContainsSynthesizedStorages \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.EpDiscoveryDetails \[$null\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.EpPolicySessionDetails \[Veeam.Backup.Model.CEpPolicySessionDetails\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.EpPolicySessionDetails.Serialize()  Def [void Serialize(System.Xml.XmlNode rootNode)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.EpPolicySessionDetails.ConfigurationSent \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.GuestIndexingComplete \[System.Boolean\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.HvDatastoreUsages \[$null\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.IsLatencyThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.NoRetry \[System.Boolean\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.OibId \[System.Guid\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.PlatformSpecificInfo \[Veeam.Backup.Common.CDomContainer\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.PlatformSpecificInfo.Clone()  Def [Veeam.Backup.Common.CDomContainer Clone()]
* $VBRBackupSessionTaskSession.Info.WorkDetails.PlatformSpecificInfo.GetObjectData()  Def [void GetObjectData(System.Runtime.Serialization.SerializationInfo info, System.Runtime.Serialization.StreamingContext context), void ISerializable.GetObjectData(System.Runtime.Serialization.SerializationInfo info, System.Runtime.Serialization.StreamingContext context)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.PlatformSpecificInfo.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRBackupSessionTaskSession.Info.WorkDetails.PlatformSpecificInfo.Serialize()  Def [string Serialize()]
* $VBRBackupSessionTaskSession.Info.WorkDetails.PlatformSpecificInfo.RootNode \[System.Xml.XmlElement\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.RepositoryId \[System.Guid\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SourceProxyId \[System.Guid\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.SourceProxyMode \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.SourceReportedFailoverToNbd \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.SourceRepositoryId \[System.Guid\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.TargetProxyId \[System.Guid\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.TargetProxyMode \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.TargetReportedFailoverToNbd \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.TaskAlgorithm \[Veeam.Backup.Model.ETaskAlgorithm\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.TaskAlgorithm.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.Info.WorkDetails.ViDatastoreUsages \[$null\] \($null\)
* $VBRBackupSessionTaskSession.Info.WorkDetails.WorkDuration \[System.TimeSpan\]
* $VBRBackupSessionTaskSession.IsFsAwareInfoLoadFailed \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobName \[System.String\]
* $VBRBackupSessionTaskSession.JobSess \[Veeam.Backup.Core.CBackupSession\]
* $VBRBackupSessionTaskSession.JobSess.AbortSession()  Def [void AbortSession()]
* $VBRBackupSessionTaskSession.JobSess.CalcBaseSessionResult()  Def [Veeam.Backup.Model.CBaseSessionInfo+EResult CalcBaseSessionResult()]
* $VBRBackupSessionTaskSession.JobSess.CalcSessionResult()  Def [Veeam.Backup.Model.CBaseSessionInfo+EResult CalcSessionResult()]
* $VBRBackupSessionTaskSession.JobSess.CanBeEncrypted()  Def [bool CanBeEncrypted(), bool IEncryptedBackupSession.CanBeEncrypted()]
* $VBRBackupSessionTaskSession.JobSess.CanDelete()  Def [bool CanDelete()]
* $VBRBackupSessionTaskSession.JobSess.CheckStop()  Def [void CheckStop(), void ISessionStopChecker.CheckStop()]
* $VBRBackupSessionTaskSession.JobSess.Complete()  Def [void Complete()]
* $VBRBackupSessionTaskSession.JobSess.CompleteBase()  Def [void CompleteBase()]
* $VBRBackupSessionTaskSession.JobSess.CompleteUncompletedTasks()  Def [void CompleteUncompletedTasks(System.Exception ex, System.Collections.Generic.IEnumerable[Veeam.Backup.Core.ITask] tasks)]
* $VBRBackupSessionTaskSession.JobSess.CompleteWithFailure()  Def [void CompleteWithFailure()]
* $VBRBackupSessionTaskSession.JobSess.CompleteWithResult()  Def [void CompleteWithResult(Veeam.Backup.Model.CBaseSessionInfo+EResult result, Veeam.Backup.Common.ETaskLogRecordStatus status)]
* $VBRBackupSessionTaskSession.JobSess.CompleteWithSuccess()  Def [void CompleteWithSuccess()]
* $VBRBackupSessionTaskSession.JobSess.CompleteWithWarning()  Def [void CompleteWithWarning()]
* $VBRBackupSessionTaskSession.JobSess.CreateNotifyHelper()  Def [Veeam.Backup.Core.CEventNotifier CreateNotifyHelper(System.Nullable[Veeam.Backup.Common.EPlatform] platform, string vmId, string uniqueHash, guid taskSessionId, string objectDisplayName)]
* $VBRBackupSessionTaskSession.JobSess.CreateTaskSession()  Def [Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom, Veeam.Backup.Core.IXmlLogger logger), Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom), Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, guid objectId, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom), Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, guid objectId, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom, string formattedIpAddress), Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, guid objectId, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom, datetime queuedTime), Veeam.Backup.Core.CBackupTaskSession CreateTaskSession(string objectName, guid objectId, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatfrom, datetime queuedTime, string formattedIpAddress)]
* $VBRBackupSessionTaskSession.JobSess.DataBagAddSafe()  Def [void DataBagAddSafe(string key, System.Object value)]
* $VBRBackupSessionTaskSession.JobSess.DataBagContainsKey()  Def [bool DataBagContainsKey(string key)]
* $VBRBackupSessionTaskSession.JobSess.DataBagGetOrAddNew()  Def [T DataBagGetOrAddNew[T](string key)]
* $VBRBackupSessionTaskSession.JobSess.DataBagGetSafe()  Def [T DataBagGetSafe[T](string key, T defaultValue)]
* $VBRBackupSessionTaskSession.JobSess.FindCreationTimeUtc()  Def [System.Nullable[datetime] FindCreationTimeUtc()]
* $VBRBackupSessionTaskSession.JobSess.FindEpPolicyContext()  Def [Veeam.Backup.Core.CEpPolicyJobSessionContext FindEpPolicyContext()]
* $VBRBackupSessionTaskSession.JobSess.FindEpRescanExcludedObjects()  Def [Veeam.Backup.Model.CEpRescanExcludedObjectsInfo FindEpRescanExcludedObjects()]
* $VBRBackupSessionTaskSession.JobSess.FindJob()  Def [Veeam.Backup.Core.CBackupJob FindJob()]
* $VBRBackupSessionTaskSession.JobSess.FindJobStartupSpec()  Def [Veeam.Backup.Model.IJobStartupSpec FindJobStartupSpec()]
* $VBRBackupSessionTaskSession.JobSess.FindObject()  Def [Veeam.Backup.Core.IHierarchyObj FindObject(guid objectId)]
* $VBRBackupSessionTaskSession.JobSess.FindOrCreateTaskSession()  Def [Veeam.Backup.Core.CBackupTaskSession FindOrCreateTaskSession(string taskSessName, guid objectId, System.Nullable[Veeam.Backup.Common.EPlatform] objectPlatform)]
* $VBRBackupSessionTaskSession.JobSess.FindSessionStarterInfo()  Def [Veeam.Backup.Model.CSessionStarterInfo FindSessionStarterInfo()]
* $VBRBackupSessionTaskSession.JobSess.FindTaskSession()  Def [Veeam.Backup.Core.CBackupTaskSession FindTaskSession(string taskSessName, guid objectId)]
* $VBRBackupSessionTaskSession.JobSess.FindTaskSessionByObjectId()  Def [Veeam.Backup.Core.CBackupTaskSession FindTaskSessionByObjectId(guid objectId)]
* $VBRBackupSessionTaskSession.JobSess.ForceSetDbMethods()  Def [void ForceSetDbMethods(Veeam.Backup.Core.IDbMethodsInterceptor dbMethods)]
* $VBRBackupSessionTaskSession.JobSess.FreezeEncryptionState()  Def [void FreezeEncryptionState()]
* $VBRBackupSessionTaskSession.JobSess.GetBackup()  Def [Veeam.Backup.Model.CBackupInfo GetBackup(Veeam.Backup.Core.IDbMethodsInterceptor interceptor), Veeam.Backup.Model.CBackupInfo IDbEncryptionSession.GetBackup(Veeam.Backup.Core.IDbMethodsInterceptor interceptor)]
* $VBRBackupSessionTaskSession.JobSess.GetBackupStats()  Def [Veeam.Backup.Model.CBackupStats GetBackupStats()]
* $VBRBackupSessionTaskSession.JobSess.GetChildSessions()  Def [Veeam.Backup.Model.CBackupSessionInfo[] GetChildSessions()]
* $VBRBackupSessionTaskSession.JobSess.GetDetails()  Def [string GetDetails()]
* $VBRBackupSessionTaskSession.JobSess.GetFullLogsSubfolder()  Def [Veeam.Backup.Common.CPath GetFullLogsSubfolder(Params string[] children)]
* $VBRBackupSessionTaskSession.JobSess.GetJob()  Def [Veeam.Backup.Core.CBackupJob GetJob()]
* $VBRBackupSessionTaskSession.JobSess.GetLastUsedCryptoKey()  Def [Veeam.Backup.Core.CCryptoKey GetLastUsedCryptoKey()]
* $VBRBackupSessionTaskSession.JobSess.GetOriginalAndRetrySessions()  Def [System.Collections.Generic.IEnumerable[Veeam.Backup.Core.CBackupSession] GetOriginalAndRetrySessions(bool forwardOrdered)]
* $VBRBackupSessionTaskSession.JobSess.GetRetrySessionModeString()  Def [string GetRetrySessionModeString()]
* $VBRBackupSessionTaskSession.JobSess.GetTaskSessions()  Def [Veeam.Backup.Core.CBackupTaskSession[] GetTaskSessions()]
* $VBRBackupSessionTaskSession.JobSess.GetTaskSessionsByStatus()  Def [Veeam.Backup.Core.CBackupTaskSession[] GetTaskSessionsByStatus(Params Veeam.Backup.Model.ESessionStatus[] statuses)]
* $VBRBackupSessionTaskSession.JobSess.IncrementTotals()  Def [void IncrementTotals(int totalObjects, long totalSize, long totalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.IsCloudConnected()  Def [bool IsCloudConnected()]
* $VBRBackupSessionTaskSession.JobSess.IsPrevOrOriginalSessHaveRecheckError()  Def [bool IsPrevOrOriginalSessHaveRecheckError()]
* $VBRBackupSessionTaskSession.JobSess.IsSessionNotHeldByJobProcess()  Def [bool IsSessionNotHeldByJobProcess()]
* $VBRBackupSessionTaskSession.JobSess.IsStoped()  Def [bool IsStoped([ref] string stopDetails), bool IsStoped([ref] string stopDetails, bool bNoLogStopSignal), bool IsStoped(), bool ISessionStopChecker.IsStoped([ref] string stopDetails)]
* $VBRBackupSessionTaskSession.JobSess.LogAndSetOperation()  Def [void LogAndSetOperation(string format, Params string[] args)]
* $VBRBackupSessionTaskSession.JobSess.OnSchedulerLoggerCreated()  Def [void OnSchedulerLoggerCreated(Veeam.Backup.Core.CTaskSchedulerSessionLogger taskSchedulerSessionLogger)]
* $VBRBackupSessionTaskSession.JobSess.ReloadSafe()  Def [void ReloadSafe()]
* $VBRBackupSessionTaskSession.JobSess.SaveJobProgress()  Def [void SaveJobProgress(), void SaveJobProgress(Veeam.Backup.Common.LogLevels logLevel)]
* $VBRBackupSessionTaskSession.JobSess.SaveJobProgressExceptObjects()  Def [void SaveJobProgressExceptObjects(Veeam.Backup.Common.LogLevels logLevels)]
* $VBRBackupSessionTaskSession.JobSess.SaveJobProgressOnlyObjects()  Def [void SaveJobProgressOnlyObjects(Veeam.Backup.Common.LogLevels logLevel)]
* $VBRBackupSessionTaskSession.JobSess.SendJobFinishEvent()  Def [void SendJobFinishEvent()]
* $VBRBackupSessionTaskSession.JobSess.SetAuxData()  Def [void SetAuxData(string auxData)]
* $VBRBackupSessionTaskSession.JobSess.SetDbMethods()  Def [void SetDbMethods(Veeam.Backup.Core.IDbMethodsInterceptor dbMethods)]
* $VBRBackupSessionTaskSession.JobSess.SetFullMode()  Def [void SetFullMode(bool setActiveFull), void SetFullMode(bool setActiveFull, bool resetPerVmEnabled)]
* $VBRBackupSessionTaskSession.JobSess.SetLeaseId()  Def [void SetLeaseId(guid leaseId)]
* $VBRBackupSessionTaskSession.JobSess.SetNonPersistentJob()  Def [void SetNonPersistentJob(Veeam.Backup.Core.CBackupJob job)]
* $VBRBackupSessionTaskSession.JobSess.SetOperation()  Def [void SetOperation(string format, Params System.Object[] args), void SetOperation(string operation)]
* $VBRBackupSessionTaskSession.JobSess.SetOriginalSessionId()  Def [void SetOriginalSessionId(guid origSessId)]
* $VBRBackupSessionTaskSession.JobSess.SetProgress()  Def [void SetProgress(int progress)]
* $VBRBackupSessionTaskSession.JobSess.SetResult()  Def [void SetResult(Veeam.Backup.Model.CBaseSessionInfo+EResult result), void SetResult(Veeam.Backup.Model.CBaseSessionInfo+EResult result, string resultDescription)]
* $VBRBackupSessionTaskSession.JobSess.SetRetryPrediction()  Def [void SetRetryPrediction(bool willBeRetried)]
* $VBRBackupSessionTaskSession.JobSess.SetSpec()  Def [void SetSpec(string spec)]
* $VBRBackupSessionTaskSession.JobSess.SetState()  Def [void SetState(Veeam.Backup.Model.CBaseSessionInfo+EState state), void IBaseSession.SetState(Veeam.Backup.Model.CBaseSessionInfo+EState state)]
* $VBRBackupSessionTaskSession.JobSess.SetTotals()  Def [void SetTotals(int totalObjects, long totalSize, long totalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.ShouldForceFullBackupByEncriptionEnablingChanging()  Def [bool ShouldForceFullBackupByEncriptionEnablingChanging()]
* $VBRBackupSessionTaskSession.JobSess.TrySetStateStopping()  Def [bool TrySetStateStopping()]
* $VBRBackupSessionTaskSession.JobSess.UpdateEpPolicyContext()  Def [void UpdateEpPolicyContext(Veeam.Backup.Core.CEpPolicyJobSessionContext context)]
* $VBRBackupSessionTaskSession.JobSess.UpdateInnerState()  Def [void UpdateInnerState()]
* $VBRBackupSessionTaskSession.JobSess.UpdateSessionAlgorithm()  Def [void UpdateSessionAlgorithm(Veeam.Backup.Model.SessionAlgorithms sessionAlgorithm)]
* $VBRBackupSessionTaskSession.JobSess.UpdateSessionStarterInfo()  Def [void UpdateSessionStarterInfo(Veeam.Backup.Model.CSessionStarterInfo starterInfo)]
* $VBRBackupSessionTaskSession.JobSess.UpdateStats()  Def [void UpdateStats(Veeam.Backup.Model.CBackupStats stats)]
* $VBRBackupSessionTaskSession.JobSess.AuxData \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.BackupStats \[Veeam.Backup.Model.CBackupStats\]
* $VBRBackupSessionTaskSession.JobSess.BackupStats.GetCompressX()  Def [double GetCompressX()]
* $VBRBackupSessionTaskSession.JobSess.BackupStats.GetDedupeX()  Def [double GetDedupeX()]
* $VBRBackupSessionTaskSession.JobSess.BackupStats.SetData()  Def [void SetData(long backupSize, long dataSize, int dedupRatio, int compressRatio)]
* $VBRBackupSessionTaskSession.JobSess.BackupStats.BackupSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.BackupStats.CompressRatio \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.BackupStats.DataSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.BackupStats.DedupRatio \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.BackupVerificationResult \[Veeam.Backup.Core.CBackupVerificationResultContainer\]
* $VBRBackupSessionTaskSession.JobSess.BackupVerificationResult.GetForStorageGroup()  Def [Veeam.Backup.Core.CStorageVerificationResultContainer GetForStorageGroup(guid objectId)]
* $VBRBackupSessionTaskSession.JobSess.BackupVerificationResult.SetForStorageGroup()  Def [void SetForStorageGroup(guid objectId, System.Collections.Generic.IEnumerable[Veeam.Backup.Core.CStorageVerificationAlg+CStorageVerificationResult] storageVerificationResults)]
* $VBRBackupSessionTaskSession.JobSess.BaseProgress \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.BottleneckManager \[CJobBottleneckManager\]
* $VBRBackupSessionTaskSession.JobSess.BottleneckManager.CalcBottleneck()  Def [Veeam.Backup.Model.EBottleneck CalcBottleneck(Veeam.Backup.Model.CBottleneckInfo bottleneckInfo)]
* $VBRBackupSessionTaskSession.JobSess.BottleneckManager.NetworkThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.BottleneckManager.RepositoryReadThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.BottleneckManager.RepositoryWriteThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.CreationTime \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.CreationTimeUTC \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.CurrentPointId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.DataBag \[System.Collections.Generic.Dictionary`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[System.Object, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\]
* $VBRBackupSessionTaskSession.JobSess.DataBag.Add()  Def [void Add(string key, System.Object value), void IDictionary[string,Object].Add(string key, System.Object value), void ICollection[KeyValuePair[string,Object]].Add(System.Collections.Generic.KeyValuePair[string,System.Object] item), void IDictionary.Add(System.Object key, System.Object value)]
* $VBRBackupSessionTaskSession.JobSess.DataBag.Clear()  Def [void Clear(), void ICollection[KeyValuePair[string,Object]].Clear(), void IDictionary.Clear()]
* $VBRBackupSessionTaskSession.JobSess.DataBag.Contains()  Def [bool ICollection[KeyValuePair[string,Object]].Contains(System.Collections.Generic.KeyValuePair[string,System.Object] item), bool IDictionary.Contains(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.DataBag.ContainsKey()  Def [bool ContainsKey(string key), bool IDictionary[string,Object].ContainsKey(string key), bool IReadOnlyDictionary[string,Object].ContainsKey(string key)]
* $VBRBackupSessionTaskSession.JobSess.DataBag.ContainsValue()  Def [bool ContainsValue(System.Object value)]
* $VBRBackupSessionTaskSession.JobSess.DataBag.CopyTo()  Def [void ICollection[KeyValuePair[string,Object]].CopyTo(System.Collections.Generic.KeyValuePair[string,System.Object][] array, int arrayIndex), void ICollection.CopyTo(array array, int index)]
* $VBRBackupSessionTaskSession.JobSess.DataBag.GetEnumerator()  Def [System.Collections.Generic.Dictionary`2+Enumerator[string,System.Object] GetEnumerator(), System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,System.Object]] IEnumerable[KeyValuePair[string,Object]].GetEnumerator(), System.Collections.IEnumerator IEnumerable.GetEnumerator(), System.Collections.IDictionaryEnumerator IDictionary.GetEnumerator()]
* $VBRBackupSessionTaskSession.JobSess.DataBag.GetObjectData()  Def [void GetObjectData(System.Runtime.Serialization.SerializationInfo info, System.Runtime.Serialization.StreamingContext context), void ISerializable.GetObjectData(System.Runtime.Serialization.SerializationInfo info, System.Runtime.Serialization.StreamingContext context)]
* $VBRBackupSessionTaskSession.JobSess.DataBag.OnDeserialization()  Def [void OnDeserialization(System.Object sender), void IDeserializationCallback.OnDeserialization(System.Object sender)]
* $VBRBackupSessionTaskSession.JobSess.DataBag.Remove()  Def [bool Remove(string key), bool IDictionary[string,Object].Remove(string key), bool ICollection[KeyValuePair[string,Object]].Remove(System.Collections.Generic.KeyValuePair[string,System.Object] item), void IDictionary.Remove(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.DataBag.TryGetValue()  Def [bool TryGetValue(string key, [ref] System.Object value), bool IDictionary[string,Object].TryGetValue(string key, [ref] System.Object value), bool IReadOnlyDictionary[string,Object].TryGetValue(string key, [ref] System.Object value)]
* $VBRBackupSessionTaskSession.JobSess.DataBag.Comparer \[System.Collections.Generic.GenericEqualityComparer`1[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\]
* $VBRBackupSessionTaskSession.JobSess.DataBag.Count \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.DataBag.IsFixedSize \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.DataBag.IsReadOnly \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.DataBag.IsSynchronized \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.DataBag.Keys \[System.Collections.Generic.Dictionary`2+KeyCollection[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[System.Object, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.DataBag.SyncRoot \[System.Object\]
* $VBRBackupSessionTaskSession.JobSess.DataBag.Values \[System.Collections.Generic.Dictionary`2+ValueCollection[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[System.Object, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Description \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.EndTime \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.EndTimeUTC \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.EventNotifier \[Veeam.Backup.Core.CEventNotifier\]
* $VBRBackupSessionTaskSession.JobSess.EventNotifier.CompleteSession()  Def [void CompleteSession()]
* $VBRBackupSessionTaskSession.JobSess.EventNotifier.CreateProgress()  Def [Veeam.Backup.Core.CEventNotifierEntry CreateProgress(Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSessionTaskSession.JobSess.EventNotifier.Notify()  Def [void Notify(Veeam.Backup.Common.ETaskLogRecordStatus status, Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSessionTaskSession.JobSess.EventNotifier.NotifySafe()  Def [void NotifySafe(Veeam.Backup.Model.CSessionEventDescriptor descriptor, Veeam.Backup.Model.CSessionEventBinding binding, Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSessionTaskSession.JobSess.EventNotifier.StartNotifyProgress()  Def [Veeam.Backup.Core.CProgressNotifyHelper StartNotifyProgress(Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSessionTaskSession.JobSess.Id \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.Info \[Veeam.Backup.Model.CBackupSessionInfo\]
* $VBRBackupSessionTaskSession.JobSess.Info.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRBackupSessionTaskSession.JobSess.Info.SetJobAlgorithm()  Def [void SetJobAlgorithm(Veeam.Backup.Model.JobAlgorithms algorithm)]
* $VBRBackupSessionTaskSession.JobSess.Info.SetSessionAlgorithm()  Def [void SetSessionAlgorithm(Veeam.Backup.Model.SessionAlgorithms algorithm)]
* $VBRBackupSessionTaskSession.JobSess.Info.AuxData \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.Info.BackedUpSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.BackupTotalSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.CompletionPercentage \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.CreationTime \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.Info.CurrentPointId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.Info.Description \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.EndTime \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.Info.Failures \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Id \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.Info.Initiator \[Veeam.Backup.Model.CBaseSessionInfo+SInitiator\]
* $VBRBackupSessionTaskSession.JobSess.Info.Initiator.Name \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Initiator.Sid \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Initiator2 \[Veeam.Backup.Model.CModifiedUserInfo\]
* $VBRBackupSessionTaskSession.JobSess.Info.Initiator2.Serialize()  Def [string Serialize(), void Serialize(System.Xml.XmlNode node)]
* $VBRBackupSessionTaskSession.JobSess.Info.Initiator2.FullName \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Initiator2.LoginType \[Veeam.Backup.Model.EModifiedUserType\]
* $VBRBackupSessionTaskSession.JobSess.Info.Initiator2.LoginType.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.IsActiveFullMode \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.IsCompleted \[System.Boolean\]
* $VBRBackupSessionTaskSession.JobSess.Info.IsFullMode \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.IsRecheckRetry \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.IsRetryMode \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.IsWorking \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.JobAlgorithm \[Veeam.Backup.Model.JobAlgorithms\]
* $VBRBackupSessionTaskSession.JobSess.Info.JobAlgorithm.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.JobId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.Info.JobName \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.Info.JobSourceType \[Veeam.Backup.Model.CDbBackupJobInfo+ESourceType\]
* $VBRBackupSessionTaskSession.JobSess.Info.JobSourceType.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.JobSpec \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.JobType \[Veeam.Backup.Model.EDbJobType\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.LeaseId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.Info.LogsSubFolder \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Operation \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.OriginalSessionId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.Info.ParentSessionId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.Info.Platform \[Veeam.Backup.Common.CPlatform\]
* $VBRBackupSessionTaskSession.JobSess.Info.Platform.IsExternalInfrastructure()  Def [bool IsExternalInfrastructure()]
* $VBRBackupSessionTaskSession.JobSess.Info.Platform.IsWellKnown()  Def [bool IsWellKnown()]
* $VBRBackupSessionTaskSession.JobSess.Info.Platform.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRBackupSessionTaskSession.JobSess.Info.Platform.Platform \[Veeam.Backup.Common.EPlatform\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Platform.PlatformId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.Info.PolicyName \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.PolicyTag \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress \[Veeam.Backup.Model.CBackupProgressData\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.AddChildAndGet()  Def [Veeam.Backup.Model.CBackupProgressData AddChildAndGet(System.Object key, Veeam.Backup.Model.CBackupProgressData child)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.ApplyUpdates()  Def [void ApplyUpdates(Veeam.Backup.Model.CBackupProgressUpdates updates)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.CalcAvgSpeed()  Def [void CalcAvgSpeed()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.CalcPercents()  Def [void CalcPercents()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Clone()  Def [Veeam.Backup.Model.CBackupProgressData Clone()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.ConvertForeignTimeToLocal()  Def [void ConvertForeignTimeToLocal(timespan timeShift)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.DecrementProcessedSize()  Def [void DecrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.DecrementTotalObjects()  Def [void DecrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.DecrementTotalSize()  Def [void DecrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.FindChild()  Def [Veeam.Backup.Model.CBackupProgressData FindChild(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.GetProcessingDuration()  Def [timespan GetProcessingDuration()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.GetRemainingTime()  Def [timespan GetRemainingTime(System.Nullable[long] avgSpeed)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.IncrementProcessedObjects()  Def [void IncrementProcessedObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.IncrementProcessedSize()  Def [void IncrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.IncrementTotalObjects()  Def [void IncrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.IncrementTotalObjectsWithProcessed()  Def [void IncrementTotalObjectsWithProcessed(int newObjects)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.IncrementTotalSize()  Def [void IncrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.IncrementTotalSizeWithProcessed()  Def [void IncrementTotalSizeWithProcessed(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.RemoveChild()  Def [void RemoveChild(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Serialize()  Def [string Serialize()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Start()  Def [void Start()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Stop()  Def [void Stop(System.Nullable[datetime] stopTime)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.UpdateBottleneck()  Def [void UpdateBottleneck(Veeam.Backup.Model.CBottleneckInfo bottleneckInfo)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.UpdateParentTotalSize()  Def [void UpdateParentTotalSize()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.UpdateParentTotalSizeIfZero()  Def [void UpdateParentTotalSizeIfZero()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.UpdateProcessedObjects()  Def [void UpdateProcessedObjects(int processedObjects)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.UpdateProcessedSize()  Def [void UpdateProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.UpdateTime()  Def [void UpdateTime(datetime startTime, datetime stopTime)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.UpdateTotalObjects()  Def [void UpdateTotalObjects(int totalObjects)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.UpdateTotalSize()  Def [void UpdateTotalSize(long totalSize, long totalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.AvgSpeed \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo \[Veeam.Backup.Model.CBottleneckInfo\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.CalcBottleneck()  Def [Veeam.Backup.Model.EBottleneck CalcBottleneck(bool networkThrottlingEnabled, bool targetRepositoryThrottlingEnabled, bool sourceRepositoryThrottlingEnabled)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.GetSettedValues()  Def [System.Tuple[string,int][] GetSettedValues()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.Serial()  Def [void Serial(System.Xml.XmlNode rootNode)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.Update()  Def [void Update(Veeam.Backup.Model.CBottleneckInfo other)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.Bottleneck \[Veeam.Backup.Model.EBottleneck\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.Network \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.NetworkThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.Proxy \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.RepositoryThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.Source \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.SourceNetwork \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.SourceProxy \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.SourceStorage \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.SourceWan \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.Target \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.TargetNetwork \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.TargetProxy \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.TargetStorage \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.BottleneckInfo.TargetWan \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Duration \[System.TimeSpan\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.IsNeedSubstractReadDelay \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Percents \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.ProcessedDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.ProcessedObjects \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.ProcessedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.ProcessedUsedDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.ProcessedUsedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.ReadedAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.ReadedAverageSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.ReadSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.StartTimeLocal \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.StartTimeUtc \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.StopTimeLocal \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.StopTimeUtc \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.TotalObjects \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.TotalSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.TotalSizeDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.TotalUsedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.TotalUsedSizeDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.TransferedDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.TransferedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates \[Veeam.Backup.Model.CBackupProgressUpdates\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.IncrementProcessedDeltas()  Def [void IncrementProcessedDeltas(long processedDeltaIncrement, long processedUsedDeltaIncrement, long readDeltaIncrement, long readAverageDeltaIncrement, long transferredDeltaIncrement)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.IncrementTotalSizeDeltas()  Def [void IncrementTotalSizeDeltas(long totalSizeDeltaIncrement, long totalUsedSizeDeltaIncrement)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.Reset()  Def [void Reset()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.SetChildBottlenecks()  Def [void SetChildBottlenecks(System.Collections.Generic.IDictionary[string,Veeam.Backup.Model.CBottleneckInfo] childBottlenecks)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.SetChildProcessingIntervals()  Def [void SetChildProcessingIntervals(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Common.CDateTimeInterval][] childIntervals)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks \[System.Collections.Concurrent.ConcurrentDictionary`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.Add()  Def [void IDictionary[string,CBottleneckInfo].Add(string key, Veeam.Backup.Model.CBottleneckInfo value), void ICollection[KeyValuePair[string,CBottleneckInfo]].Add(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Add(System.Object key, System.Object value)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.AddOrUpdate()  Def [Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, Veeam.Backup.Model.CBottleneckInfo addValue, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,TArg,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory, TArg factoryArgument)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.Clear()  Def [void Clear(), void ICollection[KeyValuePair[string,CBottleneckInfo]].Clear(), void IDictionary.Clear()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.Contains()  Def [bool ICollection[KeyValuePair[string,CBottleneckInfo]].Contains(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), bool IDictionary.Contains(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.ContainsKey()  Def [bool ContainsKey(string key), bool IDictionary[string,CBottleneckInfo].ContainsKey(string key), bool IReadOnlyDictionary[string,CBottleneckInfo].ContainsKey(string key)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.CopyTo()  Def [void ICollection[KeyValuePair[string,CBottleneckInfo]].CopyTo(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo][] array, int arrayIndex), void ICollection.CopyTo(array array, int index)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.GetEnumerator()  Def [System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] GetEnumerator(), System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] IEnumerable[KeyValuePair[string,CBottleneckInfo]].GetEnumerator(), System.Collections.IEnumerator IEnumerable.GetEnumerator(), System.Collections.IDictionaryEnumerator IDictionary.GetEnumerator()]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.GetOrAdd()  Def [Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] valueFactory), Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, Veeam.Backup.Model.CBottleneckInfo value), Veeam.Backup.Model.CBottleneckInfo GetOrAdd[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] valueFactory, TArg factoryArgument)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.Remove()  Def [bool IDictionary[string,CBottleneckInfo].Remove(string key), bool ICollection[KeyValuePair[string,CBottleneckInfo]].Remove(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Remove(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.TryAdd()  Def [bool TryAdd(string key, Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.TryGetValue()  Def [bool TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IReadOnlyDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.TryRemove()  Def [bool TryRemove(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.TryUpdate()  Def [bool TryUpdate(string key, Veeam.Backup.Model.CBottleneckInfo newValue, Veeam.Backup.Model.CBottleneckInfo comparisonValue)]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.Count \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.IsEmpty \[System.Boolean\]
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.IsFixedSize \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.IsReadOnly \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.IsSynchronized \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.Keys \[System.Collections.ObjectModel.ReadOnlyCollection`1[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.SyncRoot \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildBottlenecks.Values \[System.Collections.ObjectModel.ReadOnlyCollection`1[[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ChildProcessingIntervals \[System.Collections.Generic.KeyValuePair`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Common.CDateTimeInterval, Veeam.Backup.Common, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]][]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ReadAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.Updates.TransferredDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.Progress.UsedSpaceRation \[System.Double\]
* $VBRBackupSessionTaskSession.JobSess.Info.Result \[Veeam.Backup.Model.CBaseSessionInfo+EResult\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.RunManually \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.SessionAlgorithm \[Veeam.Backup.Model.SessionAlgorithms\]
* $VBRBackupSessionTaskSession.JobSess.Info.SessionAlgorithm.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.State \[Veeam.Backup.Model.CBaseSessionInfo+EState\]
* $VBRBackupSessionTaskSession.JobSess.Info.State.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.TransportType \[Veeam.Backup.Model.ETransportType\]
* $VBRBackupSessionTaskSession.JobSess.Info.TransportType.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Info.Warnings \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Info.WillBeRetried \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsCompleted \[System.Boolean\]
* $VBRBackupSessionTaskSession.JobSess.IsEncryptionEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsEncryptionEnabledByOptions \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsEpAgentManagement \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsFullMode \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsLowerAgentPriority \[System.Boolean\]
* $VBRBackupSessionTaskSession.JobSess.IsManuallyStopped \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsPlannedFailover \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsPostprocessing \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsQuickBackup \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsRecheckRetry \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsReplicaFromBackup \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsRetryMode \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsStarting \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsTransformLaunched \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsVeeamZip \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.IsWorking \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.JobId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.JobName \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.JobSourceType \[Veeam.Backup.Model.CDbBackupJobInfo+ESourceType\]
* $VBRBackupSessionTaskSession.JobSess.JobSourceType.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.JobSpec \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.JobType \[Veeam.Backup.Model.EDbJobType\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.JobTypeString \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.LastProgressSaveTime \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.LeaseId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.Logger \[Veeam.Backup.Core.XmlLogger\]
* $VBRBackupSessionTaskSession.JobSess.Logger.AddErr()  Def [uint64 AddErr(System.Exception exception, string title, Params System.Object[] args), uint64 AddErr(System.Exception exception, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 AddErr(System.Exception exception, string title), uint64 AddErr(string format, Params System.Object[] args), uint64 IXmlLogger.AddErr(System.Exception excSrc, string title, Params System.Object[] args), uint64 IXmlLogger.AddErr(System.Exception excSrc, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddErr(System.Exception excSrc, string title), uint64 IXmlLogger.AddErr(string format, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.JobSess.Logger.AddLog()  Def [uint64 AddLog(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, Params System.Object[] args), uint64 AddLog(string format, Params System.Object[] args), uint64 AddLog(Veeam.Backup.Common.CTaskLogRecord logRecord), uint64 IXmlLogger.AddLog(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, Params System.Object[] args), uint64 IXmlLogger.AddLog(string format, Params System.Object[] args), uint64 IXmlLogger.AddLog(Veeam.Backup.Common.CTaskLogRecord logRecord)]
* $VBRBackupSessionTaskSession.JobSess.Logger.AddLogWithDescription()  Def [uint64 AddLogWithDescription(datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility), uint64 AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, Veeam.Backup.Common.ETaskLogStyle style, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility), uint64 IXmlLogger.AddLogWithDescription(datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility), uint64 IXmlLogger.AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, Veeam.Backup.Common.ETaskLogStyle style, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility)]
* $VBRBackupSessionTaskSession.JobSess.Logger.AddOrUpdateLog()  Def [void AddOrUpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord), void IXmlLogger.AddOrUpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord)]
* $VBRBackupSessionTaskSession.JobSess.Logger.AddSuccess()  Def [uint64 AddSuccess(string title, Params System.Object[] args), uint64 AddSuccess(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 AddSuccess(string title), uint64 IXmlLogger.AddSuccess(string title, Params System.Object[] args), uint64 IXmlLogger.AddSuccess(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddSuccess(string title)]
* $VBRBackupSessionTaskSession.JobSess.Logger.AddWarning()  Def [uint64 AddWarning(string title, Params System.Object[] args), uint64 AddWarning(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 AddWarning(System.Exception exception, string title, Params System.Object[] args), uint64 AddWarning(System.Exception exception, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(System.Exception ex, string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(System.Exception ex, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.JobSess.Logger.AddWarningWithDescription()  Def [uint64 AddWarningWithDescription(System.Exception exception, string title, string desc), uint64 IXmlLogger.AddWarningWithDescription(System.Exception ex, string title, string desc)]
* $VBRBackupSessionTaskSession.JobSess.Logger.ChangeStatus()  Def [void ChangeStatus(Veeam.Backup.Common.ETaskLogRecordStatus fromStatus, Veeam.Backup.Common.ETaskLogRecordStatus toStatus), void IXmlLogger.ChangeStatus(Veeam.Backup.Common.ETaskLogRecordStatus fromStatus, Veeam.Backup.Common.ETaskLogRecordStatus toStatus)]
* $VBRBackupSessionTaskSession.JobSess.Logger.Clear()  Def [void Clear(), void IXmlLogger.Clear()]
* $VBRBackupSessionTaskSession.JobSess.Logger.Complete()  Def [void Complete(string[] cookies, Veeam.Backup.Common.ETaskLogRecordStatus status), void Complete(string[] cookies, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status), void Complete(string[] cookiesArray, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string description), void Complete(string[] cookiesArray, Veeam.Backup.Common.ETaskLogRecordStatus status, string description), void Complete(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status), void Complete(string cookie, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status), void IXmlLogger.Complete(string[] cookies, Veeam.Backup.Common.ETaskLogRecordStatus status), void IXmlLogger.Complete(string[] cookies, Veeam.Backup.Common.ETaskLogRecordStatus status, string description), void IXmlLogger.Complete(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status)]
* $VBRBackupSessionTaskSession.JobSess.Logger.CompleteAll()  Def [void CompleteAll(Veeam.Backup.Common.ETaskLogRecordStatus status, string description), void IXmlLogger.CompleteAll(Veeam.Backup.Common.ETaskLogRecordStatus status, string description)]
* $VBRBackupSessionTaskSession.JobSess.Logger.CompleteSuccess()  Def [void CompleteSuccess(string cookie), void CompleteSuccess(string cookie, datetime time), void IXmlLogger.CompleteSuccess(string cookie), void IXmlLogger.CompleteSuccess(string cookie, datetime time)]
* $VBRBackupSessionTaskSession.JobSess.Logger.GetLog()  Def [Veeam.Backup.Common.CTaskLogUpdates GetLog(uint64 usn), Veeam.Backup.Common.CTaskLogUpdates GetLog(), Veeam.Backup.Common.CTaskLogUpdates IXmlLogger.GetLog(), Veeam.Backup.Common.CTaskLogUpdates IXmlLogger.GetLog(uint64 usn)]
* $VBRBackupSessionTaskSession.JobSess.Logger.GetMaxSeverity()  Def [Veeam.Backup.Common.ETaskLogRecordStatus GetMaxSeverity(), Veeam.Backup.Common.ETaskLogRecordStatus IXmlLogger.GetMaxSeverity()]
* $VBRBackupSessionTaskSession.JobSess.Logger.GetRecordIdByCookieOrNull()  Def [System.Nullable[uint64] GetRecordIdByCookieOrNull(string cookie), System.Nullable[uint64] IXmlLogger.GetRecordIdByCookieOrNull(string cookie)]
* $VBRBackupSessionTaskSession.JobSess.Logger.GetTopUsn()  Def [uint64 GetTopUsn(), uint64 IXmlLogger.GetTopUsn()]
* $VBRBackupSessionTaskSession.JobSess.Logger.IsRecordExistWithCookie()  Def [bool IsRecordExistWithCookie(string cookie), bool IXmlLogger.IsRecordExistWithCookie(string cookie)]
* $VBRBackupSessionTaskSession.JobSess.Logger.RemoveRecord()  Def [uint64 RemoveRecord(uint64 logRecordId), uint64 IXmlLogger.RemoveRecord(uint64 logRecordId)]
* $VBRBackupSessionTaskSession.JobSess.Logger.RemoveRecords()  Def [uint64 RemoveRecords(uint64 firstLogRecordId, uint64 lastLogRecordId), uint64 IXmlLogger.RemoveRecords(uint64 firstLogRecordId, uint64 lastLogRecordId)]
* $VBRBackupSessionTaskSession.JobSess.Logger.SetErr()  Def [uint64 SetErr(string cookie, System.Exception exception, string title, Params System.Object[] args), uint64 SetErr(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetErr(string cookie, System.Exception ex, string title, Params System.Object[] args), uint64 IXmlLogger.SetErr(string cookie, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.JobSess.Logger.SetInProgress()  Def [uint64 SetInProgress(string cookie, string title, Params System.Object[] args), uint64 SetInProgress(string cookie, datetime time, string title, Params System.Object[] args), uint64 IXmlLogger.SetInProgress(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetInProgress(string cookie, datetime time, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.JobSess.Logger.SetSuccess()  Def [uint64 SetSuccess(string cookie, string title, Params System.Object[] args), uint64 SetSuccess(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.SetSuccess(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetSuccess(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.JobSess.Logger.SetWarning()  Def [uint64 SetWarning(string cookie, System.Exception exception, string title, Params System.Object[] args), uint64 SetWarning(string cookie, string title, Params System.Object[] args), uint64 SetWarning(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.SetWarning(string cookie, System.Exception ex, string title, Params System.Object[] args), uint64 IXmlLogger.SetWarning(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetWarning(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.JobSess.Logger.TryGetLog()  Def [bool TryGetLog(uint64 usn, [ref] Veeam.Backup.Common.CTaskLogUpdates updates), bool IXmlLogGetter.TryGetLog(uint64 usn, [ref] Veeam.Backup.Common.CTaskLogUpdates updates)]
* $VBRBackupSessionTaskSession.JobSess.Logger.UpdateErr()  Def [uint64 UpdateErr(uint64 logRecordId, string title, System.Exception exception), uint64 UpdateErr(uint64 logRecordId, string title), void UpdateErr(uint64 logRecordId), uint64 IXmlLogger.UpdateErr(uint64 logRecordId, string title, System.Exception ex), uint64 IXmlLogger.UpdateErr(uint64 logRecordId, string title), void IXmlLogger.UpdateErr(uint64 logRecordId)]
* $VBRBackupSessionTaskSession.JobSess.Logger.UpdateLog()  Def [uint64 UpdateLog(uint64 logRecordId, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 UpdateLog(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 UpdateLog(uint64 logRecordId, string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 UpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord), uint64 IXmlLogger.UpdateLog(uint64 logRecordId, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.UpdateLog(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.UpdateLog(uint64 logRecordId, string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.UpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord)]
* $VBRBackupSessionTaskSession.JobSess.Logger.UpdateStatus()  Def [void UpdateStatus(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status), void IXmlLogger.UpdateStatus(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status)]
* $VBRBackupSessionTaskSession.JobSess.Logger.UpdateSuccess()  Def [uint64 UpdateSuccess(uint64 logRecordId, string title), uint64 IXmlLogger.UpdateSuccess(uint64 logRecordId, string title)]
* $VBRBackupSessionTaskSession.JobSess.Logger.UpdateWarning()  Def [uint64 UpdateWarning(uint64 logRecordId, string title), uint64 UpdateWarning(uint64 logRecordId, string title, System.Exception exception), uint64 IXmlLogger.UpdateWarning(uint64 logRecordId, string title), uint64 IXmlLogger.UpdateWarning(uint64 logRecordId, string title, System.Exception ex)]
* $VBRBackupSessionTaskSession.JobSess.Logger.Formatter \[Veeam.Backup.Core.XmlLoggerFormatter\]
* $VBRBackupSessionTaskSession.JobSess.Logger.Formatter.FormatErrorNoThrow()  Def [string FormatErrorNoThrow(bool isError, System.Exception exception, string title, Params System.Object[] args), string IXmlLoggerFormatter.FormatErrorNoThrow(bool isError, System.Exception exception, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.JobSess.Logger.Formatter.FormatNoThrow()  Def [string FormatNoThrow(string title, System.Object[] args), string IXmlLoggerFormatter.FormatNoThrow(string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.JobSess.Logger.MinTimeout \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Logger.SessionId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.Logger.Token \[Veeam.Backup.Model.CXmlLogToken\]
* $VBRBackupSessionTaskSession.JobSess.Logger.Token.FormatterType \[Veeam.Backup.Model.EXmlFormatterType\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Logger.Token.IsNullLogToken \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Logger.Token.SessId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.LogName \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.LogsSubFolder \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.MasterKey \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Name \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.Operation \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.OriginalSessionId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.OrigJobName \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.ParentSessionId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.PostActivity \[Veeam.Backup.Core.CBackupSession+EPostActivity\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress \[Veeam.Backup.Model.CBackupProgressData\]
* $VBRBackupSessionTaskSession.JobSess.Progress.AddChildAndGet()  Def [Veeam.Backup.Model.CBackupProgressData AddChildAndGet(System.Object key, Veeam.Backup.Model.CBackupProgressData child)]
* $VBRBackupSessionTaskSession.JobSess.Progress.ApplyUpdates()  Def [void ApplyUpdates(Veeam.Backup.Model.CBackupProgressUpdates updates)]
* $VBRBackupSessionTaskSession.JobSess.Progress.CalcAvgSpeed()  Def [void CalcAvgSpeed()]
* $VBRBackupSessionTaskSession.JobSess.Progress.CalcPercents()  Def [void CalcPercents()]
* $VBRBackupSessionTaskSession.JobSess.Progress.Clone()  Def [Veeam.Backup.Model.CBackupProgressData Clone()]
* $VBRBackupSessionTaskSession.JobSess.Progress.ConvertForeignTimeToLocal()  Def [void ConvertForeignTimeToLocal(timespan timeShift)]
* $VBRBackupSessionTaskSession.JobSess.Progress.DecrementProcessedSize()  Def [void DecrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.JobSess.Progress.DecrementTotalObjects()  Def [void DecrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.JobSess.Progress.DecrementTotalSize()  Def [void DecrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.Progress.FindChild()  Def [Veeam.Backup.Model.CBackupProgressData FindChild(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.Progress.GetProcessingDuration()  Def [timespan GetProcessingDuration()]
* $VBRBackupSessionTaskSession.JobSess.Progress.GetRemainingTime()  Def [timespan GetRemainingTime(System.Nullable[long] avgSpeed)]
* $VBRBackupSessionTaskSession.JobSess.Progress.IncrementProcessedObjects()  Def [void IncrementProcessedObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.JobSess.Progress.IncrementProcessedSize()  Def [void IncrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.JobSess.Progress.IncrementTotalObjects()  Def [void IncrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.JobSess.Progress.IncrementTotalObjectsWithProcessed()  Def [void IncrementTotalObjectsWithProcessed(int newObjects)]
* $VBRBackupSessionTaskSession.JobSess.Progress.IncrementTotalSize()  Def [void IncrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.Progress.IncrementTotalSizeWithProcessed()  Def [void IncrementTotalSizeWithProcessed(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.Progress.RemoveChild()  Def [void RemoveChild(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Serialize()  Def [string Serialize()]
* $VBRBackupSessionTaskSession.JobSess.Progress.Start()  Def [void Start()]
* $VBRBackupSessionTaskSession.JobSess.Progress.Stop()  Def [void Stop(System.Nullable[datetime] stopTime)]
* $VBRBackupSessionTaskSession.JobSess.Progress.UpdateBottleneck()  Def [void UpdateBottleneck(Veeam.Backup.Model.CBottleneckInfo bottleneckInfo)]
* $VBRBackupSessionTaskSession.JobSess.Progress.UpdateParentTotalSize()  Def [void UpdateParentTotalSize()]
* $VBRBackupSessionTaskSession.JobSess.Progress.UpdateParentTotalSizeIfZero()  Def [void UpdateParentTotalSizeIfZero()]
* $VBRBackupSessionTaskSession.JobSess.Progress.UpdateProcessedObjects()  Def [void UpdateProcessedObjects(int processedObjects)]
* $VBRBackupSessionTaskSession.JobSess.Progress.UpdateProcessedSize()  Def [void UpdateProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.JobSess.Progress.UpdateTime()  Def [void UpdateTime(datetime startTime, datetime stopTime)]
* $VBRBackupSessionTaskSession.JobSess.Progress.UpdateTotalObjects()  Def [void UpdateTotalObjects(int totalObjects)]
* $VBRBackupSessionTaskSession.JobSess.Progress.UpdateTotalSize()  Def [void UpdateTotalSize(long totalSize, long totalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.Progress.AvgSpeed \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo \[Veeam.Backup.Model.CBottleneckInfo\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.CalcBottleneck()  Def [Veeam.Backup.Model.EBottleneck CalcBottleneck(bool networkThrottlingEnabled, bool targetRepositoryThrottlingEnabled, bool sourceRepositoryThrottlingEnabled)]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.GetSettedValues()  Def [System.Tuple[string,int][] GetSettedValues()]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.Serial()  Def [void Serial(System.Xml.XmlNode rootNode)]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.Update()  Def [void Update(Veeam.Backup.Model.CBottleneckInfo other)]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.Bottleneck \[Veeam.Backup.Model.EBottleneck\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.Network \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.NetworkThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.Proxy \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.RepositoryThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.Source \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.SourceNetwork \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.SourceProxy \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.SourceStorage \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.SourceWan \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.Target \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.TargetNetwork \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.TargetProxy \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.TargetStorage \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.BottleneckInfo.TargetWan \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.Duration \[System.TimeSpan\]
* $VBRBackupSessionTaskSession.JobSess.Progress.IsNeedSubstractReadDelay \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Percents \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.ProcessedDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.ProcessedObjects \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.ProcessedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.ProcessedUsedDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.ProcessedUsedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.ReadedAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.ReadedAverageSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.ReadSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.StartTimeLocal \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.Progress.StartTimeUtc \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.Progress.StopTimeLocal \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.Progress.StopTimeUtc \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.Progress.TotalObjects \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Progress.TotalSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.TotalSizeDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.TotalUsedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.TotalUsedSizeDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.TransferedDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.TransferedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates \[Veeam.Backup.Model.CBackupProgressUpdates\]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.IncrementProcessedDeltas()  Def [void IncrementProcessedDeltas(long processedDeltaIncrement, long processedUsedDeltaIncrement, long readDeltaIncrement, long readAverageDeltaIncrement, long transferredDeltaIncrement)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.IncrementTotalSizeDeltas()  Def [void IncrementTotalSizeDeltas(long totalSizeDeltaIncrement, long totalUsedSizeDeltaIncrement)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.Reset()  Def [void Reset()]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.SetChildBottlenecks()  Def [void SetChildBottlenecks(System.Collections.Generic.IDictionary[string,Veeam.Backup.Model.CBottleneckInfo] childBottlenecks)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.SetChildProcessingIntervals()  Def [void SetChildProcessingIntervals(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Common.CDateTimeInterval][] childIntervals)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks \[System.Collections.Concurrent.ConcurrentDictionary`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.Add()  Def [void IDictionary[string,CBottleneckInfo].Add(string key, Veeam.Backup.Model.CBottleneckInfo value), void ICollection[KeyValuePair[string,CBottleneckInfo]].Add(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Add(System.Object key, System.Object value)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.AddOrUpdate()  Def [Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, Veeam.Backup.Model.CBottleneckInfo addValue, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,TArg,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory, TArg factoryArgument)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.Clear()  Def [void Clear(), void ICollection[KeyValuePair[string,CBottleneckInfo]].Clear(), void IDictionary.Clear()]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.Contains()  Def [bool ICollection[KeyValuePair[string,CBottleneckInfo]].Contains(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), bool IDictionary.Contains(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.ContainsKey()  Def [bool ContainsKey(string key), bool IDictionary[string,CBottleneckInfo].ContainsKey(string key), bool IReadOnlyDictionary[string,CBottleneckInfo].ContainsKey(string key)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.CopyTo()  Def [void ICollection[KeyValuePair[string,CBottleneckInfo]].CopyTo(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo][] array, int arrayIndex), void ICollection.CopyTo(array array, int index)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.GetEnumerator()  Def [System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] GetEnumerator(), System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] IEnumerable[KeyValuePair[string,CBottleneckInfo]].GetEnumerator(), System.Collections.IEnumerator IEnumerable.GetEnumerator(), System.Collections.IDictionaryEnumerator IDictionary.GetEnumerator()]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.GetOrAdd()  Def [Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] valueFactory), Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, Veeam.Backup.Model.CBottleneckInfo value), Veeam.Backup.Model.CBottleneckInfo GetOrAdd[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] valueFactory, TArg factoryArgument)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.Remove()  Def [bool IDictionary[string,CBottleneckInfo].Remove(string key), bool ICollection[KeyValuePair[string,CBottleneckInfo]].Remove(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Remove(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.TryAdd()  Def [bool TryAdd(string key, Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.TryGetValue()  Def [bool TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IReadOnlyDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.TryRemove()  Def [bool TryRemove(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.TryUpdate()  Def [bool TryUpdate(string key, Veeam.Backup.Model.CBottleneckInfo newValue, Veeam.Backup.Model.CBottleneckInfo comparisonValue)]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.Count \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.IsEmpty \[System.Boolean\]
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.IsFixedSize \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.IsReadOnly \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.IsSynchronized \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.Keys \[System.Collections.ObjectModel.ReadOnlyCollection`1[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.SyncRoot \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildBottlenecks.Values \[System.Collections.ObjectModel.ReadOnlyCollection`1[[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ChildProcessingIntervals \[System.Collections.Generic.KeyValuePair`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Common.CDateTimeInterval, Veeam.Backup.Common, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]][]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ReadAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.Updates.TransferredDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.Progress.UsedSpaceRation \[System.Double\]
* $VBRBackupSessionTaskSession.JobSess.Result \[Veeam.Backup.Model.CBaseSessionInfo+EResult\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SelectiveProcessingSpec \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec \[Veeam.Backup.Crypto.CCryptoSymmetricSpec\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.CloneWithouKeys()  Def [Veeam.Backup.Crypto.CCryptoSymmetricSpec CloneWithouKeys()]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.CloneWithoutKeys()  Def [Veeam.Backup.Crypto.ICryptoSpec ICryptoSpec.CloneWithoutKeys()]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.CloneWithoutRepair()  Def [Veeam.Backup.Crypto.CCryptoSymmetricSpec CloneWithoutRepair()]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.CreateRecoveryRecord()  Def [void CreateRecoveryRecord(Veeam.Backup.Crypto.CCryptoSymmetricSpec child), void ICryptoSpec.CreateRecoveryRecord(Veeam.Backup.Crypto.CCryptoSymmetricSpec child)]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Decrypt()  Def [byte[] Decrypt(byte[] bytes)]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.DecryptString()  Def [string DecryptString(string str)]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Dispose()  Def [void Dispose(), void IDisposable.Dispose()]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Encrypt()  Def [byte[] Encrypt(byte[] bytes)]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.EncryptString()  Def [string EncryptString(string str)]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.RecoverKeys()  Def [void RecoverKeys(Veeam.Backup.Crypto.CCryptoSymmetricSpec child)]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.CreationTime \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.CryptoAlg \[Veeam.Backup.Crypto.ECryptoAlg\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.CryptoAlg.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Hint \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Id \[Veeam.Backup.Model.CKeySetId\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Id.IsEqual()  Def [bool IsEqual(Veeam.Backup.Model.CKeySetId keySetId)]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Id.IsEmpty \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Id.Value \[System.Byte[]\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.KeyValue \[Veeam.Backup.Model.CKeyBlob\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.KeyValue.Dispose()  Def [void Dispose(), void IDisposable.Dispose()]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.KeyValue.IsNullOrEmpty()  Def [bool IsNullOrEmpty()]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.KeyValue.Raw \[System.Byte[]\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Raw \[Veeam.Backup.Model.CSerializedKeySet\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Raw.AsBase64()  Def [string AsBase64()]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Raw.Serialize()  Def [string Serialize(), void Serialize(System.Xml.XmlNode node)]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Raw.IsEmpty \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.Raw.Raw \[System.Byte[]\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.RepairRecs \[Veeam.Backup.Model.CRepairRec[]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.UsageRole \[Veeam.Backup.Crypto.ECryptoUsageRole\]
* $VBRBackupSessionTaskSession.JobSess.SessionCryptoSpec.UsageRole.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo \[Veeam.Backup.Model.CBackupSessionInfo\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.SetJobAlgorithm()  Def [void SetJobAlgorithm(Veeam.Backup.Model.JobAlgorithms algorithm)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.SetSessionAlgorithm()  Def [void SetSessionAlgorithm(Veeam.Backup.Model.SessionAlgorithms algorithm)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.AuxData \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.BackedUpSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.BackupTotalSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.CompletionPercentage \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.CreationTime \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.CurrentPointId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Description \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.EndTime \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Failures \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Id \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Initiator \[Veeam.Backup.Model.CBaseSessionInfo+SInitiator\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Initiator.Name \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Initiator.Sid \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Initiator2 \[Veeam.Backup.Model.CModifiedUserInfo\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Initiator2.Serialize()  Def [string Serialize(), void Serialize(System.Xml.XmlNode node)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Initiator2.FullName \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Initiator2.LoginType \[Veeam.Backup.Model.EModifiedUserType\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Initiator2.LoginType.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.IsActiveFullMode \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.IsCompleted \[System.Boolean\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.IsFullMode \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.IsRecheckRetry \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.IsRetryMode \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.IsWorking \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.JobAlgorithm \[Veeam.Backup.Model.JobAlgorithms\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.JobAlgorithm.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.JobId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.JobName \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.JobSourceType \[Veeam.Backup.Model.CDbBackupJobInfo+ESourceType\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.JobSourceType.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.JobSpec \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.JobType \[Veeam.Backup.Model.EDbJobType\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.LeaseId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.LogsSubFolder \[System.String\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Operation \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.OriginalSessionId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.ParentSessionId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Platform \[Veeam.Backup.Common.CPlatform\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Platform.IsExternalInfrastructure()  Def [bool IsExternalInfrastructure()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Platform.IsWellKnown()  Def [bool IsWellKnown()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Platform.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Platform.Platform \[Veeam.Backup.Common.EPlatform\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Platform.PlatformId \[System.Guid\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.PolicyName \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.PolicyTag \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress \[Veeam.Backup.Model.CBackupProgressData\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.AddChildAndGet()  Def [Veeam.Backup.Model.CBackupProgressData AddChildAndGet(System.Object key, Veeam.Backup.Model.CBackupProgressData child)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.ApplyUpdates()  Def [void ApplyUpdates(Veeam.Backup.Model.CBackupProgressUpdates updates)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.CalcAvgSpeed()  Def [void CalcAvgSpeed()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.CalcPercents()  Def [void CalcPercents()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Clone()  Def [Veeam.Backup.Model.CBackupProgressData Clone()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.ConvertForeignTimeToLocal()  Def [void ConvertForeignTimeToLocal(timespan timeShift)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.DecrementProcessedSize()  Def [void DecrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.DecrementTotalObjects()  Def [void DecrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.DecrementTotalSize()  Def [void DecrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.FindChild()  Def [Veeam.Backup.Model.CBackupProgressData FindChild(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.GetProcessingDuration()  Def [timespan GetProcessingDuration()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.GetRemainingTime()  Def [timespan GetRemainingTime(System.Nullable[long] avgSpeed)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.IncrementProcessedObjects()  Def [void IncrementProcessedObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.IncrementProcessedSize()  Def [void IncrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.IncrementTotalObjects()  Def [void IncrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.IncrementTotalObjectsWithProcessed()  Def [void IncrementTotalObjectsWithProcessed(int newObjects)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.IncrementTotalSize()  Def [void IncrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.IncrementTotalSizeWithProcessed()  Def [void IncrementTotalSizeWithProcessed(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.RemoveChild()  Def [void RemoveChild(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Serialize()  Def [string Serialize()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Start()  Def [void Start()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Stop()  Def [void Stop(System.Nullable[datetime] stopTime)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.UpdateBottleneck()  Def [void UpdateBottleneck(Veeam.Backup.Model.CBottleneckInfo bottleneckInfo)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.UpdateParentTotalSize()  Def [void UpdateParentTotalSize()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.UpdateParentTotalSizeIfZero()  Def [void UpdateParentTotalSizeIfZero()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.UpdateProcessedObjects()  Def [void UpdateProcessedObjects(int processedObjects)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.UpdateProcessedSize()  Def [void UpdateProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.UpdateTime()  Def [void UpdateTime(datetime startTime, datetime stopTime)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.UpdateTotalObjects()  Def [void UpdateTotalObjects(int totalObjects)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.UpdateTotalSize()  Def [void UpdateTotalSize(long totalSize, long totalUsedSize)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.AvgSpeed \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo \[Veeam.Backup.Model.CBottleneckInfo\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.CalcBottleneck()  Def [Veeam.Backup.Model.EBottleneck CalcBottleneck(bool networkThrottlingEnabled, bool targetRepositoryThrottlingEnabled, bool sourceRepositoryThrottlingEnabled)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.GetSettedValues()  Def [System.Tuple[string,int][] GetSettedValues()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.Serial()  Def [void Serial(System.Xml.XmlNode rootNode)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.Update()  Def [void Update(Veeam.Backup.Model.CBottleneckInfo other)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.Bottleneck \[Veeam.Backup.Model.EBottleneck\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.Network \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.NetworkThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.Proxy \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.RepositoryThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.Source \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.SourceNetwork \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.SourceProxy \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.SourceStorage \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.SourceWan \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.Target \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.TargetNetwork \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.TargetProxy \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.TargetStorage \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.BottleneckInfo.TargetWan \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Duration \[System.TimeSpan\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.IsNeedSubstractReadDelay \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Percents \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.ProcessedDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.ProcessedObjects \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.ProcessedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.ProcessedUsedDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.ProcessedUsedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.ReadedAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.ReadedAverageSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.ReadSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.StartTimeLocal \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.StartTimeUtc \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.StopTimeLocal \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.StopTimeUtc \[System.DateTime\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.TotalObjects \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.TotalSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.TotalSizeDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.TotalUsedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.TotalUsedSizeDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.TransferedDelta \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.TransferedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates \[Veeam.Backup.Model.CBackupProgressUpdates\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.IncrementProcessedDeltas()  Def [void IncrementProcessedDeltas(long processedDeltaIncrement, long processedUsedDeltaIncrement, long readDeltaIncrement, long readAverageDeltaIncrement, long transferredDeltaIncrement)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.IncrementTotalSizeDeltas()  Def [void IncrementTotalSizeDeltas(long totalSizeDeltaIncrement, long totalUsedSizeDeltaIncrement)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.Reset()  Def [void Reset()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.SetChildBottlenecks()  Def [void SetChildBottlenecks(System.Collections.Generic.IDictionary[string,Veeam.Backup.Model.CBottleneckInfo] childBottlenecks)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.SetChildProcessingIntervals()  Def [void SetChildProcessingIntervals(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Common.CDateTimeInterval][] childIntervals)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks \[System.Collections.Concurrent.ConcurrentDictionary`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.Add()  Def [void IDictionary[string,CBottleneckInfo].Add(string key, Veeam.Backup.Model.CBottleneckInfo value), void ICollection[KeyValuePair[string,CBottleneckInfo]].Add(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Add(System.Object key, System.Object value)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.AddOrUpdate()  Def [Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, Veeam.Backup.Model.CBottleneckInfo addValue, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,TArg,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory, TArg factoryArgument)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.Clear()  Def [void Clear(), void ICollection[KeyValuePair[string,CBottleneckInfo]].Clear(), void IDictionary.Clear()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.Contains()  Def [bool ICollection[KeyValuePair[string,CBottleneckInfo]].Contains(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), bool IDictionary.Contains(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.ContainsKey()  Def [bool ContainsKey(string key), bool IDictionary[string,CBottleneckInfo].ContainsKey(string key), bool IReadOnlyDictionary[string,CBottleneckInfo].ContainsKey(string key)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.CopyTo()  Def [void ICollection[KeyValuePair[string,CBottleneckInfo]].CopyTo(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo][] array, int arrayIndex), void ICollection.CopyTo(array array, int index)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.GetEnumerator()  Def [System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] GetEnumerator(), System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] IEnumerable[KeyValuePair[string,CBottleneckInfo]].GetEnumerator(), System.Collections.IEnumerator IEnumerable.GetEnumerator(), System.Collections.IDictionaryEnumerator IDictionary.GetEnumerator()]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.GetOrAdd()  Def [Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] valueFactory), Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, Veeam.Backup.Model.CBottleneckInfo value), Veeam.Backup.Model.CBottleneckInfo GetOrAdd[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] valueFactory, TArg factoryArgument)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.Remove()  Def [bool IDictionary[string,CBottleneckInfo].Remove(string key), bool ICollection[KeyValuePair[string,CBottleneckInfo]].Remove(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Remove(System.Object key)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.TryAdd()  Def [bool TryAdd(string key, Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.TryGetValue()  Def [bool TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IReadOnlyDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.TryRemove()  Def [bool TryRemove(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.TryUpdate()  Def [bool TryUpdate(string key, Veeam.Backup.Model.CBottleneckInfo newValue, Veeam.Backup.Model.CBottleneckInfo comparisonValue)]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.Count \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.IsEmpty \[System.Boolean\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.IsFixedSize \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.IsReadOnly \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.IsSynchronized \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.Keys \[System.Collections.ObjectModel.ReadOnlyCollection`1[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.SyncRoot \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildBottlenecks.Values \[System.Collections.ObjectModel.ReadOnlyCollection`1[[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ChildProcessingIntervals \[System.Collections.Generic.KeyValuePair`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Common.CDateTimeInterval, Veeam.Backup.Common, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]][]\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ReadAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.Updates.TransferredDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Progress.UsedSpaceRation \[System.Double\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Result \[Veeam.Backup.Model.CBaseSessionInfo+EResult\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.RunManually \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.SessionAlgorithm \[Veeam.Backup.Model.SessionAlgorithms\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.SessionAlgorithm.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.State \[Veeam.Backup.Model.CBaseSessionInfo+EState\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.State.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.TransportType \[Veeam.Backup.Model.ETransportType\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.TransportType.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.Warnings \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SessionInfo.WillBeRetried \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.SplitStoragesPerVm \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.StartupMode \[Veeam.Backup.Model.CDbBackupJobInfo+Mode\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.State \[Veeam.Backup.Model.CBaseSessionInfo+EState\]
* $VBRBackupSessionTaskSession.JobSess.State.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.JobSess.Tracer \[Veeam.Backup.Core.CSessionLogTracer\]
* $VBRBackupSessionTaskSession.JobSess.Tracer.TraceError()  Def [void TraceError(), void TraceError(string formatMsg, Params string[] args)]
* $VBRBackupSessionTaskSession.JobSess.Tracer.TraceException()  Def [void TraceException(System.Exception excSrc), void ILogTracer.TraceException(System.Exception excSrc)]
* $VBRBackupSessionTaskSession.JobSess.Tracer.TraceIfDifferentText()  Def [void TraceIfDifferentText(string formatMsg, Params string[] args)]
* $VBRBackupSessionTaskSession.JobSess.Tracer.TraceNext()  Def [void TraceNext(Veeam.Backup.Common.ELogRecordVisibility visibility, string formatMsg, Params string[] args), void TraceNext(string formatMsg, Params string[] args), void ILogTracer.TraceNext(string formatMsg, Params string[] args), void ILogTracer.TraceNext(Veeam.Backup.Common.ELogRecordVisibility visibility, string formatMsg, Params string[] args)]
* $VBRBackupSessionTaskSession.JobSess.Tracer.TraceOk()  Def [void TraceOk(), void ILogTracer.TraceOk()]
* $VBRBackupSessionTaskSession.JobSess.Tracer.TraceWarning()  Def [void TraceWarning(), void TraceWarning(string formatMsg, Params string[] args)]
* $VBRBackupSessionTaskSession.JobSess.UserCryptoSpec \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.UserKey \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.WillBeRetried \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.WorkDetails \[Veeam.Backup.Core.CBackupSessionWorkDetails\]
* $VBRBackupSessionTaskSession.JobSess.WorkDetails.GetRecheckInfo()  Def [Veeam.Backup.Core.CBackupSessionRecheckInfo GetRecheckInfo()]
* $VBRBackupSessionTaskSession.JobSess.WorkDetails.RecheckInfo \[$null\] \($null\)
* $VBRBackupSessionTaskSession.JobSess.WorkDetails.WorkDuration \[System.TimeSpan\]
* $VBRBackupSessionTaskSession.JobSessId \[System.Guid\]
* $VBRBackupSessionTaskSession.Logger \[Veeam.Backup.Core.XmlLoggerCumulative\]
* $VBRBackupSessionTaskSession.Logger.AddErr()  Def [uint64 AddErr(System.Exception excSrc, string title, Params System.Object[] args), uint64 AddErr(System.Exception excSrc, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 AddErr(System.Exception excSrc, string title), uint64 AddErr(string title, Params System.Object[] args), uint64 IXmlLogger.AddErr(System.Exception excSrc, string title, Params System.Object[] args), uint64 IXmlLogger.AddErr(System.Exception excSrc, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddErr(System.Exception excSrc, string title), uint64 IXmlLogger.AddErr(string format, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.Logger.AddErrorCumulativeMessage()  Def [uint64 AddErrorCumulativeMessage(string cumulativeString, string format, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.Logger.AddLog()  Def [uint64 AddLog(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, Params System.Object[] args), uint64 AddLog(string format, Params System.Object[] args), uint64 AddLog(Veeam.Backup.Common.CTaskLogRecord logRecord), uint64 IXmlLogger.AddLog(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, Params System.Object[] args), uint64 IXmlLogger.AddLog(string format, Params System.Object[] args), uint64 IXmlLogger.AddLog(Veeam.Backup.Common.CTaskLogRecord logRecord)]
* $VBRBackupSessionTaskSession.Logger.AddLogOrRefreshCumulativeCount()  Def [uint64 AddLogOrRefreshCumulativeCount(Veeam.Backup.Common.ETaskLogRecordStatus status, Veeam.Backup.Common.ETaskLogStyle style, string cumulativeString, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility)]
* $VBRBackupSessionTaskSession.Logger.AddLogWithDescription()  Def [uint64 AddLogWithDescription(datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility), uint64 AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, Veeam.Backup.Common.ETaskLogStyle style, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility), uint64 IXmlLogger.AddLogWithDescription(datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.AddLogWithDescription(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility), uint64 IXmlLogger.AddLogWithDescription(Veeam.Backup.Common.ETaskLogRecordStatus status, Veeam.Backup.Common.ETaskLogStyle style, string title, string desc, Veeam.Backup.Common.ELogRecordVisibility visibility)]
* $VBRBackupSessionTaskSession.Logger.AddOrUpdateLog()  Def [void AddOrUpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord), void IXmlLogger.AddOrUpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord)]
* $VBRBackupSessionTaskSession.Logger.AddSuccess()  Def [uint64 AddSuccess(string title, Params System.Object[] args), uint64 AddSuccess(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 AddSuccess(string title), uint64 IXmlLogger.AddSuccess(string title, Params System.Object[] args), uint64 IXmlLogger.AddSuccess(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddSuccess(string title)]
* $VBRBackupSessionTaskSession.Logger.AddSuccessCumulativeMessage()  Def [uint64 AddSuccessCumulativeMessage(string cumulativeString, string format, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.Logger.AddWarning()  Def [uint64 AddWarning(string title, Params System.Object[] args), uint64 AddWarning(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 AddWarning(System.Exception ex, string title, Params System.Object[] args), uint64 AddWarning(System.Exception ex, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(System.Exception ex, string title, Params System.Object[] args), uint64 IXmlLogger.AddWarning(System.Exception ex, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.Logger.AddWarningCumulativeMessage()  Def [uint64 AddWarningCumulativeMessage(string cumulativeString, string format, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.Logger.AddWarningWithDescription()  Def [uint64 AddWarningWithDescription(System.Exception ex, string title, string desc), uint64 IXmlLogger.AddWarningWithDescription(System.Exception ex, string title, string desc)]
* $VBRBackupSessionTaskSession.Logger.ChangeInternalLogger()  Def [void ChangeInternalLogger(Veeam.Backup.Core.IXmlLogger logger)]
* $VBRBackupSessionTaskSession.Logger.ChangeStatus()  Def [void ChangeStatus(Veeam.Backup.Common.ETaskLogRecordStatus fromStatus, Veeam.Backup.Common.ETaskLogRecordStatus toStatus), void IXmlLogger.ChangeStatus(Veeam.Backup.Common.ETaskLogRecordStatus fromStatus, Veeam.Backup.Common.ETaskLogRecordStatus toStatus)]
* $VBRBackupSessionTaskSession.Logger.Clear()  Def [void Clear(), void IXmlLogger.Clear()]
* $VBRBackupSessionTaskSession.Logger.Complete()  Def [void Complete(string[] cookies, Veeam.Backup.Common.ETaskLogRecordStatus status), void Complete(string[] cookies, Veeam.Backup.Common.ETaskLogRecordStatus status, string description), void Complete(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status), void IXmlLogger.Complete(string[] cookies, Veeam.Backup.Common.ETaskLogRecordStatus status), void IXmlLogger.Complete(string[] cookies, Veeam.Backup.Common.ETaskLogRecordStatus status, string description), void IXmlLogger.Complete(string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status)]
* $VBRBackupSessionTaskSession.Logger.CompleteAll()  Def [void CompleteAll(Veeam.Backup.Common.ETaskLogRecordStatus status, string description), void IXmlLogger.CompleteAll(Veeam.Backup.Common.ETaskLogRecordStatus status, string description)]
* $VBRBackupSessionTaskSession.Logger.CompleteSuccess()  Def [void CompleteSuccess(string cookie), void CompleteSuccess(string cookie, datetime time), void IXmlLogger.CompleteSuccess(string cookie), void IXmlLogger.CompleteSuccess(string cookie, datetime time)]
* $VBRBackupSessionTaskSession.Logger.GetExclusivePrefixDecorator()  Def [void GetExclusivePrefixDecorator(string prefix, string cookiePrefix)]
* $VBRBackupSessionTaskSession.Logger.GetLog()  Def [Veeam.Backup.Common.CTaskLogUpdates GetLog(), Veeam.Backup.Common.CTaskLogUpdates GetLog(uint64 usn), Veeam.Backup.Common.CTaskLogUpdates IXmlLogger.GetLog(), Veeam.Backup.Common.CTaskLogUpdates IXmlLogger.GetLog(uint64 usn)]
* $VBRBackupSessionTaskSession.Logger.GetMaxSeverity()  Def [Veeam.Backup.Common.ETaskLogRecordStatus GetMaxSeverity(), Veeam.Backup.Common.ETaskLogRecordStatus IXmlLogger.GetMaxSeverity()]
* $VBRBackupSessionTaskSession.Logger.GetRecordIdByCookieOrNull()  Def [System.Nullable[uint64] GetRecordIdByCookieOrNull(string cookie), System.Nullable[uint64] IXmlLogger.GetRecordIdByCookieOrNull(string cookie)]
* $VBRBackupSessionTaskSession.Logger.GetTopUsn()  Def [uint64 GetTopUsn(), uint64 IXmlLogger.GetTopUsn()]
* $VBRBackupSessionTaskSession.Logger.IsActiveMessageHaveOldPosition()  Def [bool IsActiveMessageHaveOldPosition(string cumulativeString)]
* $VBRBackupSessionTaskSession.Logger.IsMessageCumulative()  Def [bool IsMessageCumulative(string cumulativeString)]
* $VBRBackupSessionTaskSession.Logger.IsRecordExistWithCookie()  Def [bool IsRecordExistWithCookie(string cookie), bool IXmlLogger.IsRecordExistWithCookie(string cookie)]
* $VBRBackupSessionTaskSession.Logger.RefreshCumulativeActiveMessage()  Def [uint64 RefreshCumulativeActiveMessage(string cumulativeString, uint64 activeMessagePosition, Veeam.Backup.Common.ETaskLogRecordStatus taskStatus)]
* $VBRBackupSessionTaskSession.Logger.RefreshCumulativeMessage()  Def [uint64 RefreshCumulativeMessage(string cumulativeString, Veeam.Backup.Common.ETaskLogRecordStatus taskStatus)]
* $VBRBackupSessionTaskSession.Logger.RemoveRecord()  Def [uint64 RemoveRecord(uint64 logRecordId), uint64 IXmlLogger.RemoveRecord(uint64 logRecordId)]
* $VBRBackupSessionTaskSession.Logger.RemoveRecords()  Def [uint64 RemoveRecords(uint64 firstLogRecordId, uint64 lastLogRecordId), uint64 IXmlLogger.RemoveRecords(uint64 firstLogRecordId, uint64 lastLogRecordId)]
* $VBRBackupSessionTaskSession.Logger.SetErr()  Def [uint64 SetErr(string cookie, System.Exception ex, string title, Params System.Object[] args), uint64 SetErr(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetErr(string cookie, System.Exception ex, string title, Params System.Object[] args), uint64 IXmlLogger.SetErr(string cookie, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.Logger.SetInProgress()  Def [uint64 SetInProgress(string cookie, string title, Params System.Object[] args), uint64 SetInProgress(string cookie, datetime time, string title, Params System.Object[] args), uint64 IXmlLogger.SetInProgress(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetInProgress(string cookie, datetime time, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.Logger.SetSuccess()  Def [uint64 SetSuccess(string cookie, string title, Params System.Object[] args), uint64 SetSuccess(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.SetSuccess(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetSuccess(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.Logger.SetWarning()  Def [uint64 SetWarning(string cookie, System.Exception ex, string title, Params System.Object[] args), uint64 SetWarning(string cookie, string title, Params System.Object[] args), uint64 SetWarning(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args), uint64 IXmlLogger.SetWarning(string cookie, System.Exception ex, string title, Params System.Object[] args), uint64 IXmlLogger.SetWarning(string cookie, string title, Params System.Object[] args), uint64 IXmlLogger.SetWarning(string cookie, Veeam.Backup.Common.ELogRecordVisibility visibility, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.Logger.UpdateErr()  Def [uint64 UpdateErr(uint64 logRecordId, string title, System.Exception ex), uint64 UpdateErr(uint64 logRecordId, string title), void UpdateErr(uint64 logRecordId), uint64 IXmlLogger.UpdateErr(uint64 logRecordId, string title, System.Exception ex), uint64 IXmlLogger.UpdateErr(uint64 logRecordId, string title), void IXmlLogger.UpdateErr(uint64 logRecordId)]
* $VBRBackupSessionTaskSession.Logger.UpdateLog()  Def [uint64 UpdateLog(uint64 logRecordId, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 UpdateLog(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 UpdateLog(uint64 logRecordId, string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 UpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord), uint64 IXmlLogger.UpdateLog(uint64 logRecordId, datetime time, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.UpdateLog(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.UpdateLog(uint64 logRecordId, string cookie, Veeam.Backup.Common.ETaskLogRecordStatus status, string title, string desc), uint64 IXmlLogger.UpdateLog(Veeam.Backup.Common.CTaskLogRecord logRecord)]
* $VBRBackupSessionTaskSession.Logger.UpdateStatus()  Def [void UpdateStatus(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status), void IXmlLogger.UpdateStatus(uint64 logRecordId, Veeam.Backup.Common.ETaskLogRecordStatus status)]
* $VBRBackupSessionTaskSession.Logger.UpdateSuccess()  Def [uint64 UpdateSuccess(uint64 logRecordId, string title), uint64 IXmlLogger.UpdateSuccess(uint64 logRecordId, string title)]
* $VBRBackupSessionTaskSession.Logger.UpdateWarning()  Def [uint64 UpdateWarning(uint64 logRecordId, string title), uint64 UpdateWarning(uint64 logRecordId, string title, System.Exception ex), uint64 IXmlLogger.UpdateWarning(uint64 logRecordId, string title), uint64 IXmlLogger.UpdateWarning(uint64 logRecordId, string title, System.Exception ex)]
* $VBRBackupSessionTaskSession.Logger.Formatter \[Veeam.Backup.Core.XmlLoggerFormatter\]
* $VBRBackupSessionTaskSession.Logger.Formatter.FormatErrorNoThrow()  Def [string FormatErrorNoThrow(bool isError, System.Exception exception, string title, Params System.Object[] args), string IXmlLoggerFormatter.FormatErrorNoThrow(bool isError, System.Exception exception, string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.Logger.Formatter.FormatNoThrow()  Def [string FormatNoThrow(string title, System.Object[] args), string IXmlLoggerFormatter.FormatNoThrow(string title, Params System.Object[] args)]
* $VBRBackupSessionTaskSession.Logger.Token \[Veeam.Backup.Model.CXmlLogToken\]
* $VBRBackupSessionTaskSession.Logger.Token.FormatterType \[Veeam.Backup.Model.EXmlFormatterType\]
* $VBRBackupSessionTaskSession.Logger.Token.FormatterType.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.Logger.Token.IsNullLogToken \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Logger.Token.SessId \[System.Guid\]
* $VBRBackupSessionTaskSession.Name \[System.String\]
* $VBRBackupSessionTaskSession.Operation \[System.String\] \($null\)
* $VBRBackupSessionTaskSession.Progress \[Veeam.Backup.Model.CBackupProgressData\]
* $VBRBackupSessionTaskSession.Progress.AddChildAndGet()  Def [Veeam.Backup.Model.CBackupProgressData AddChildAndGet(System.Object key, Veeam.Backup.Model.CBackupProgressData child)]
* $VBRBackupSessionTaskSession.Progress.ApplyUpdates()  Def [void ApplyUpdates(Veeam.Backup.Model.CBackupProgressUpdates updates)]
* $VBRBackupSessionTaskSession.Progress.CalcAvgSpeed()  Def [void CalcAvgSpeed()]
* $VBRBackupSessionTaskSession.Progress.CalcPercents()  Def [void CalcPercents()]
* $VBRBackupSessionTaskSession.Progress.Clone()  Def [Veeam.Backup.Model.CBackupProgressData Clone()]
* $VBRBackupSessionTaskSession.Progress.ConvertForeignTimeToLocal()  Def [void ConvertForeignTimeToLocal(timespan timeShift)]
* $VBRBackupSessionTaskSession.Progress.DecrementProcessedSize()  Def [void DecrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.Progress.DecrementTotalObjects()  Def [void DecrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.Progress.DecrementTotalSize()  Def [void DecrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.Progress.FindChild()  Def [Veeam.Backup.Model.CBackupProgressData FindChild(System.Object key)]
* $VBRBackupSessionTaskSession.Progress.GetProcessingDuration()  Def [timespan GetProcessingDuration()]
* $VBRBackupSessionTaskSession.Progress.GetRemainingTime()  Def [timespan GetRemainingTime(System.Nullable[long] avgSpeed)]
* $VBRBackupSessionTaskSession.Progress.IncrementProcessedObjects()  Def [void IncrementProcessedObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.Progress.IncrementProcessedSize()  Def [void IncrementProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.Progress.IncrementTotalObjects()  Def [void IncrementTotalObjects(int deltaProcessedObjects)]
* $VBRBackupSessionTaskSession.Progress.IncrementTotalObjectsWithProcessed()  Def [void IncrementTotalObjectsWithProcessed(int newObjects)]
* $VBRBackupSessionTaskSession.Progress.IncrementTotalSize()  Def [void IncrementTotalSize(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.Progress.IncrementTotalSizeWithProcessed()  Def [void IncrementTotalSizeWithProcessed(long deltaTotalSize, long deltaTotalUsedSize)]
* $VBRBackupSessionTaskSession.Progress.RemoveChild()  Def [void RemoveChild(System.Object key)]
* $VBRBackupSessionTaskSession.Progress.Serialize()  Def [string Serialize()]
* $VBRBackupSessionTaskSession.Progress.Start()  Def [void Start()]
* $VBRBackupSessionTaskSession.Progress.Stop()  Def [void Stop(System.Nullable[datetime] stopTime)]
* $VBRBackupSessionTaskSession.Progress.UpdateBottleneck()  Def [void UpdateBottleneck(Veeam.Backup.Model.CBottleneckInfo bottleneckInfo)]
* $VBRBackupSessionTaskSession.Progress.UpdateParentTotalSize()  Def [void UpdateParentTotalSize()]
* $VBRBackupSessionTaskSession.Progress.UpdateParentTotalSizeIfZero()  Def [void UpdateParentTotalSizeIfZero()]
* $VBRBackupSessionTaskSession.Progress.UpdateProcessedObjects()  Def [void UpdateProcessedObjects(int processedObjects)]
* $VBRBackupSessionTaskSession.Progress.UpdateProcessedSize()  Def [void UpdateProcessedSize(long processedSize, long processedUsedSize, long readSize, long readedAverageSize, long transferedSize)]
* $VBRBackupSessionTaskSession.Progress.UpdateTime()  Def [void UpdateTime(datetime startTime, datetime stopTime)]
* $VBRBackupSessionTaskSession.Progress.UpdateTotalObjects()  Def [void UpdateTotalObjects(int totalObjects)]
* $VBRBackupSessionTaskSession.Progress.UpdateTotalSize()  Def [void UpdateTotalSize(long totalSize, long totalUsedSize)]
* $VBRBackupSessionTaskSession.Progress.AvgSpeed \[System.Int64\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo \[Veeam.Backup.Model.CBottleneckInfo\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.CalcBottleneck()  Def [Veeam.Backup.Model.EBottleneck CalcBottleneck(bool networkThrottlingEnabled, bool targetRepositoryThrottlingEnabled, bool sourceRepositoryThrottlingEnabled)]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.GetSettedValues()  Def [System.Tuple[string,int][] GetSettedValues()]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.Serial()  Def [void Serial(System.Xml.XmlNode rootNode)]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.Update()  Def [void Update(Veeam.Backup.Model.CBottleneckInfo other)]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.Bottleneck \[Veeam.Backup.Model.EBottleneck\] \($null\)
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.Network \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.NetworkThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.Proxy \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.RepositoryThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.Source \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.SourceNetwork \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.SourceProxy \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.SourceStorage \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.SourceWan \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.Target \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.TargetNetwork \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.TargetProxy \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.TargetStorage \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.BottleneckInfo.TargetWan \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.Duration \[System.TimeSpan\]
* $VBRBackupSessionTaskSession.Progress.IsNeedSubstractReadDelay \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Percents \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.Progress.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.ProcessedObjects \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.ProcessedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Progress.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.ProcessedUsedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Progress.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.ReadedAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.ReadedAverageSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Progress.ReadSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Progress.StartTimeLocal \[System.DateTime\]
* $VBRBackupSessionTaskSession.Progress.StartTimeUtc \[System.DateTime\]
* $VBRBackupSessionTaskSession.Progress.StopTimeLocal \[System.DateTime\]
* $VBRBackupSessionTaskSession.Progress.StopTimeUtc \[System.DateTime\]
* $VBRBackupSessionTaskSession.Progress.TotalObjects \[System.Int32\]
* $VBRBackupSessionTaskSession.Progress.TotalSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Progress.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.TotalUsedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Progress.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.TransferedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.TransferedSize \[System.Int64\]
* $VBRBackupSessionTaskSession.Progress.Updates \[Veeam.Backup.Model.CBackupProgressUpdates\]
* $VBRBackupSessionTaskSession.Progress.Updates.IncrementProcessedDeltas()  Def [void IncrementProcessedDeltas(long processedDeltaIncrement, long processedUsedDeltaIncrement, long readDeltaIncrement, long readAverageDeltaIncrement, long transferredDeltaIncrement)]
* $VBRBackupSessionTaskSession.Progress.Updates.IncrementTotalSizeDeltas()  Def [void IncrementTotalSizeDeltas(long totalSizeDeltaIncrement, long totalUsedSizeDeltaIncrement)]
* $VBRBackupSessionTaskSession.Progress.Updates.Reset()  Def [void Reset()]
* $VBRBackupSessionTaskSession.Progress.Updates.SetChildBottlenecks()  Def [void SetChildBottlenecks(System.Collections.Generic.IDictionary[string,Veeam.Backup.Model.CBottleneckInfo] childBottlenecks)]
* $VBRBackupSessionTaskSession.Progress.Updates.SetChildProcessingIntervals()  Def [void SetChildProcessingIntervals(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Common.CDateTimeInterval][] childIntervals)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks \[System.Collections.Concurrent.ConcurrentDictionary`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.Add()  Def [void IDictionary[string,CBottleneckInfo].Add(string key, Veeam.Backup.Model.CBottleneckInfo value), void ICollection[KeyValuePair[string,CBottleneckInfo]].Add(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Add(System.Object key, System.Object value)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.AddOrUpdate()  Def [Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate(string key, Veeam.Backup.Model.CBottleneckInfo addValue, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory), Veeam.Backup.Model.CBottleneckInfo AddOrUpdate[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] addValueFactory, System.Func[string,Veeam.Backup.Model.CBottleneckInfo,TArg,Veeam.Backup.Model.CBottleneckInfo] updateValueFactory, TArg factoryArgument)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.Clear()  Def [void Clear(), void ICollection[KeyValuePair[string,CBottleneckInfo]].Clear(), void IDictionary.Clear()]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.Contains()  Def [bool ICollection[KeyValuePair[string,CBottleneckInfo]].Contains(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), bool IDictionary.Contains(System.Object key)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.ContainsKey()  Def [bool ContainsKey(string key), bool IDictionary[string,CBottleneckInfo].ContainsKey(string key), bool IReadOnlyDictionary[string,CBottleneckInfo].ContainsKey(string key)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.CopyTo()  Def [void ICollection[KeyValuePair[string,CBottleneckInfo]].CopyTo(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo][] array, int arrayIndex), void ICollection.CopyTo(array array, int index)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.GetEnumerator()  Def [System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] GetEnumerator(), System.Collections.Generic.IEnumerator[System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo]] IEnumerable[KeyValuePair[string,CBottleneckInfo]].GetEnumerator(), System.Collections.IEnumerator IEnumerable.GetEnumerator(), System.Collections.IDictionaryEnumerator IDictionary.GetEnumerator()]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.GetOrAdd()  Def [Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, System.Func[string,Veeam.Backup.Model.CBottleneckInfo] valueFactory), Veeam.Backup.Model.CBottleneckInfo GetOrAdd(string key, Veeam.Backup.Model.CBottleneckInfo value), Veeam.Backup.Model.CBottleneckInfo GetOrAdd[TArg](string key, System.Func[string,TArg,Veeam.Backup.Model.CBottleneckInfo] valueFactory, TArg factoryArgument)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.Remove()  Def [bool IDictionary[string,CBottleneckInfo].Remove(string key), bool ICollection[KeyValuePair[string,CBottleneckInfo]].Remove(System.Collections.Generic.KeyValuePair[string,Veeam.Backup.Model.CBottleneckInfo] item), void IDictionary.Remove(System.Object key)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.TryAdd()  Def [bool TryAdd(string key, Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.TryGetValue()  Def [bool TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value), bool IReadOnlyDictionary[string,CBottleneckInfo].TryGetValue(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.TryRemove()  Def [bool TryRemove(string key, [ref] Veeam.Backup.Model.CBottleneckInfo value)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.TryUpdate()  Def [bool TryUpdate(string key, Veeam.Backup.Model.CBottleneckInfo newValue, Veeam.Backup.Model.CBottleneckInfo comparisonValue)]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.Count \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.IsEmpty \[System.Boolean\]
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.IsFixedSize \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.IsReadOnly \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.IsSynchronized \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.Keys \[System.Collections.ObjectModel.ReadOnlyCollection`1[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.SyncRoot \[$null\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.ChildBottlenecks.Values \[System.Collections.ObjectModel.ReadOnlyCollection`1[[Veeam.Backup.Model.CBottleneckInfo, Veeam.Backup.Model, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]]\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.ChildProcessingIntervals \[System.Collections.Generic.KeyValuePair`2[[System.String, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089],[Veeam.Backup.Common.CDateTimeInterval, Veeam.Backup.Common, Version=9.5.0.0, Culture=neutral, PublicKeyToken=bfd684de2276783a]][]\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.ProcessedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.ProcessedUsedDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.ReadAverageDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.ReadDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.TotalSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.TotalUsedSizeDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.Updates.TransferredDelta \[System.Int64\] \($null\)
* $VBRBackupSessionTaskSession.Progress.UsedSpaceRation \[System.Double\]
* $VBRBackupSessionTaskSession.ProgressManager \[Veeam.Backup.Core.CBackupTaskSessionProgress\]
* $VBRBackupSessionTaskSession.ProgressManager.ExcludeTaskFromJobProgress()  Def [void ExcludeTaskFromJobProgress()]
* $VBRBackupSessionTaskSession.ProgressManager.IncrementJobProcessedObjects()  Def [void IncrementJobProcessedObjects(int deltaProcessedObjects, Veeam.Backup.Common.LogLevels logLevel)]
* $VBRBackupSessionTaskSession.ProgressManager.IncrementTaskProcessedObjects()  Def [void IncrementTaskProcessedObjects(int deltaProcessedObjects, Veeam.Backup.Common.LogLevels logLevel)]
* $VBRBackupSessionTaskSession.ProgressManager.SetCurrentNdmpVolumeSizeAndIsNeedCorrectTotalSize()  Def [void SetCurrentNdmpVolumeSizeAndIsNeedCorrectTotalSize(long ndmpVolumeSize)]
* $VBRBackupSessionTaskSession.ProgressManager.SetTaskTotalObjects()  Def [void SetTaskTotalObjects(int totalObjects)]
* $VBRBackupSessionTaskSession.ProgressManager.SetTaskTotalSize()  Def [void SetTaskTotalSize(long totalSize, System.Nullable[long] totalUsedSize)]
* $VBRBackupSessionTaskSession.ProgressManager.UpdateFileProgress()  Def [void UpdateFileProgress(Veeam.Backup.AgentProvider.IProgressEventArgsEx arg, Veeam.Backup.Common.LogLevels logLevel)]
* $VBRBackupSessionTaskSession.ProgressManager.UpdateNdmpTaskProgress()  Def [void UpdateNdmpTaskProgress(Veeam.Backup.AgentProvider.IProgressEventArgsEx arg, Veeam.Backup.Common.LogLevels logLevel)]
* $VBRBackupSessionTaskSession.ProgressManager.UpdateTaskProgress()  Def [void UpdateTaskProgress(Veeam.Backup.AgentProvider.IProgressEventArgsEx arg, Veeam.Backup.Common.LogLevels logLevel)]
* $VBRBackupSessionTaskSession.ProgressManager.RemainingVmObjectsCount \[Veeam.Backup.Core.CBackupTaskSessionObjectsCount\]
* $VBRBackupSessionTaskSession.ProgressManager.RemainingVmObjectsCount.DecrementValue()  Def [void DecrementValue()]
* $VBRBackupSessionTaskSession.ProgressManager.RemainingVmObjectsCount.Value \[System.Int32\]
* $VBRBackupSessionTaskSession.ProgressManager._lastProgressSaveTime \[System.DateTime\]
* $VBRBackupSessionTaskSession.RetryCounter \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.Status \[Veeam.Backup.Model.ESessionStatus\] \($null\)
* $VBRBackupSessionTaskSession.StopDetails \[$null\] \($null\)
* $VBRBackupSessionTaskSession.TaskEventNotifier \[Veeam.Backup.Core.CEventNotifier\]
* $VBRBackupSessionTaskSession.TaskEventNotifier.CompleteSession()  Def [void CompleteSession()]
* $VBRBackupSessionTaskSession.TaskEventNotifier.CreateProgress()  Def [Veeam.Backup.Core.CEventNotifierEntry CreateProgress(Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSessionTaskSession.TaskEventNotifier.Notify()  Def [void Notify(Veeam.Backup.Common.ETaskLogRecordStatus status, Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSessionTaskSession.TaskEventNotifier.NotifySafe()  Def [void NotifySafe(Veeam.Backup.Model.CSessionEventDescriptor descriptor, Veeam.Backup.Model.CSessionEventBinding binding, Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSessionTaskSession.TaskEventNotifier.StartNotifyProgress()  Def [Veeam.Backup.Core.CProgressNotifyHelper StartNotifyProgress(Veeam.Backup.Model.ISessionEvent sessionEvent)]
* $VBRBackupSessionTaskSession.Tracer \[Veeam.Backup.Core.CSessionLogTracer\]
* $VBRBackupSessionTaskSession.Tracer.TraceError()  Def [void TraceError(), void TraceError(string formatMsg, Params string[] args)]
* $VBRBackupSessionTaskSession.Tracer.TraceException()  Def [void TraceException(System.Exception excSrc), void ILogTracer.TraceException(System.Exception excSrc)]
* $VBRBackupSessionTaskSession.Tracer.TraceIfDifferentText()  Def [void TraceIfDifferentText(string formatMsg, Params string[] args)]
* $VBRBackupSessionTaskSession.Tracer.TraceNext()  Def [void TraceNext(Veeam.Backup.Common.ELogRecordVisibility visibility, string formatMsg, Params string[] args), void TraceNext(string formatMsg, Params string[] args), void ILogTracer.TraceNext(string formatMsg, Params string[] args), void ILogTracer.TraceNext(Veeam.Backup.Common.ELogRecordVisibility visibility, string formatMsg, Params string[] args)]
* $VBRBackupSessionTaskSession.Tracer.TraceOk()  Def [void TraceOk(), void ILogTracer.TraceOk()]
* $VBRBackupSessionTaskSession.Tracer.TraceWarning()  Def [void TraceWarning(), void TraceWarning(string formatMsg, Params string[] args)]
* $VBRBackupSessionTaskSession.WillBeRetried \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails \[Veeam.Backup.Model.CBackupTaskWorkDetails\]
* $VBRBackupSessionTaskSession.WorkDetails.AddCreatedOib()  Def [void AddCreatedOib(guid id)]
* $VBRBackupSessionTaskSession.WorkDetails.GetCreatedOibs()  Def [guid[] GetCreatedOibs()]
* $VBRBackupSessionTaskSession.WorkDetails.RemoveCreatedOib()  Def [void RemoveCreatedOib(guid id)]
* $VBRBackupSessionTaskSession.WorkDetails.Serial()  Def [string Serial()]
* $VBRBackupSessionTaskSession.WorkDetails.SetCannotUseCBT()  Def [void SetCannotUseCBT(string reason)]
* $VBRBackupSessionTaskSession.WorkDetails.SetEpDiscoveryDetails()  Def [void SetEpDiscoveryDetails(Veeam.Backup.Model.Sources.Sessions.CEpDiscoverySessionDetails details)]
* $VBRBackupSessionTaskSession.WorkDetails.SetEpPolicyDetails()  Def [void SetEpPolicyDetails(bool configurationSent)]
* $VBRBackupSessionTaskSession.WorkDetails.SetHvDatastoreUsages()  Def [void SetHvDatastoreUsages(Veeam.Backup.Model.CHvDatastoreUsage[] hvDatastoreUsages)]
* $VBRBackupSessionTaskSession.WorkDetails.SetNoRetry()  Def [void SetNoRetry(bool value)]
* $VBRBackupSessionTaskSession.WorkDetails.SetOibInfo()  Def [void SetOibInfo(guid oibId)]
* $VBRBackupSessionTaskSession.WorkDetails.SetRepositoryInfo()  Def [void SetRepositoryInfo(guid repositoryId)]
* $VBRBackupSessionTaskSession.WorkDetails.SetSourceProxyInfo()  Def [void SetSourceProxyInfo(guid proxyId, int transportMode)]
* $VBRBackupSessionTaskSession.WorkDetails.SetSourceReportedFailoverToNbd()  Def [void SetSourceReportedFailoverToNbd()]
* $VBRBackupSessionTaskSession.WorkDetails.SetSourceRepositoryInfo()  Def [void SetSourceRepositoryInfo(guid repositoryId)]
* $VBRBackupSessionTaskSession.WorkDetails.SetTargetProxyInfo()  Def [void SetTargetProxyInfo(guid proxyId, int transportMode)]
* $VBRBackupSessionTaskSession.WorkDetails.SetTargetReportedFailoverToNbd()  Def [void SetTargetReportedFailoverToNbd()]
* $VBRBackupSessionTaskSession.WorkDetails.SetTaskAlgorithm()  Def [void SetTaskAlgorithm(Veeam.Backup.Model.ETaskAlgorithm algorithm)]
* $VBRBackupSessionTaskSession.WorkDetails.SetViDatastoreUsages()  Def [void SetViDatastoreUsages(Veeam.Backup.Model.CViDatastoreUsage[] viDatastoreUsages)]
* $VBRBackupSessionTaskSession.WorkDetails.SetWorkDuration()  Def [void SetWorkDuration(timespan workDuration)]
* $VBRBackupSessionTaskSession.WorkDetails.CannotUseCBT \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.CannotUseCBTReason \[$null\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.ContainsSynthesizedStorages \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.EpDiscoveryDetails \[$null\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.EpPolicySessionDetails \[Veeam.Backup.Model.CEpPolicySessionDetails\]
* $VBRBackupSessionTaskSession.WorkDetails.EpPolicySessionDetails.Serialize()  Def [void Serialize(System.Xml.XmlNode rootNode)]
* $VBRBackupSessionTaskSession.WorkDetails.EpPolicySessionDetails.ConfigurationSent \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.GuestIndexingComplete \[System.Boolean\]
* $VBRBackupSessionTaskSession.WorkDetails.HvDatastoreUsages \[$null\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.IsLatencyThrottlingEnabled \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.NoRetry \[System.Boolean\]
* $VBRBackupSessionTaskSession.WorkDetails.OibId \[System.Guid\]
* $VBRBackupSessionTaskSession.WorkDetails.PlatformSpecificInfo \[Veeam.Backup.Common.CDomContainer\]
* $VBRBackupSessionTaskSession.WorkDetails.PlatformSpecificInfo.Clone()  Def [Veeam.Backup.Common.CDomContainer Clone()]
* $VBRBackupSessionTaskSession.WorkDetails.PlatformSpecificInfo.GetObjectData()  Def [void GetObjectData(System.Runtime.Serialization.SerializationInfo info, System.Runtime.Serialization.StreamingContext context), void ISerializable.GetObjectData(System.Runtime.Serialization.SerializationInfo info, System.Runtime.Serialization.StreamingContext context)]
* $VBRBackupSessionTaskSession.WorkDetails.PlatformSpecificInfo.Serial()  Def [void Serial(System.Xml.XmlNode node)]
* $VBRBackupSessionTaskSession.WorkDetails.PlatformSpecificInfo.Serialize()  Def [string Serialize()]
* $VBRBackupSessionTaskSession.WorkDetails.PlatformSpecificInfo.RootNode \[System.Xml.XmlElement\]
* $VBRBackupSessionTaskSession.WorkDetails.RepositoryId \[System.Guid\]
* $VBRBackupSessionTaskSession.WorkDetails.SourceProxyId \[System.Guid\]
* $VBRBackupSessionTaskSession.WorkDetails.SourceProxyMode \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.SourceReportedFailoverToNbd \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.SourceRepositoryId \[System.Guid\]
* $VBRBackupSessionTaskSession.WorkDetails.TargetProxyId \[System.Guid\]
* $VBRBackupSessionTaskSession.WorkDetails.TargetProxyMode \[System.Int32\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.TargetReportedFailoverToNbd \[System.Boolean\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.TaskAlgorithm \[Veeam.Backup.Model.ETaskAlgorithm\]
* $VBRBackupSessionTaskSession.WorkDetails.TaskAlgorithm.value__ \[System.Int32\]
* $VBRBackupSessionTaskSession.WorkDetails.ViDatastoreUsages \[$null\] \($null\)
* $VBRBackupSessionTaskSession.WorkDetails.WorkDuration \[System.TimeSpan\]
* $VBRBackupSessionTaskSession.WorkTimer \[Veeam.Backup.Core.CBackupTaskSessionWorkTimer\]
* $VBRBackupSessionTaskSession.WorkTimer.Start()  Def [void Start()]
* $VBRBackupSessionTaskSession.WorkTimer.Stop()  Def [void Stop()]



