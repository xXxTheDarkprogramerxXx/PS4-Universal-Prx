# PS4-Universal-Prx
This is a prx to be used in unity home brew by devs who prefer c#


This project is a higly modified version of the orginal version by [RetroGamer74](https://github.com/RetroGamer74/PS4_UnjailPlugin_Unity_NativeCode)

This version does way more than just escaping sandbox 

Follow Development on [Trello](https://trello.com/c/NThzaJzZ/65-universal-plugin-for-unity)


List of functions 
```csharp
  int FreeUnjail(int FWVersion);//e.g 505
  void SetDebuggerTrue();//this prints a whole lot of notifications on the console
  int FreeFTP();//starts an ftp server
  int FreeMountUsb();
  int FreeMount();
  int GetPid();
  int GetUid();
  bool LoadExec(string path, string argv);//Luanch another application from our application
  string GetCallableList();//debug function
  string GetListOfServices()//debug funciton
  string GetIDPS();//Gets IDPS of the console using machdep
  string GetPSID();//Gets the PSID of the console
  string GetKernelVersion();//gets the kernel version
  string KernelGetOpenPsId();//gets the PSID there are two calls for some reason
  int MountSaveData(string TITLEID,string fingerprint);//mounts a selected 
  int UnMountSaveData();//required to unmount savedata if you dont unmount it will cause an app crash
  int SendMessageToPS4(string Message);//Send a notification to the ps4
  string GetUsername();//username of the current user
  string GetUserId();//gets the userid of the current urser
  int UnlockTrophies(string NPComID);//unlock a trophy with its np comid
  int Change_Controller_Color(int r,int g,int b);//change controlor color to whatever you want
  int TakeScreenShot();//saves it to /data/screenshot.png not quite sure why you would need this 
```
