# CobaltStrike BOF
Collection of beacon BOF.

# 1 ) DCOM Lateral Movement
A quick PoC that uses DCOM (ShellWindows) via beacon object files for lateral movement.You can either specify credentials or use the current user. To use the current user, just leave the domain, username, and password empty. A short article can be about using COM objects in C [can be found here](https://yaxser.github.io/CobaltStrike-BOF/).
      
# 2 ) WMI Lateral Movement - Win32_Process Create 
Similar concepts to the previous one, but an interesting learning experince. Code adopted from [CIA Vault 8](https://wikileaks.org/ciav7p1/cms/page_11628905.html). This method uses the class Win32_Process.

# 3 ) WMI Lateral Movement - Event Subscription
This one uses WMI events for lateral movement. Most of the heavy lifting was done by [wumb0in](https://wumb0.in/scheduling-callbacks-with-wmi-in-cpp.html)


## Why are you doing this?
I ported these techniques to BOF in order to learn more about Windows, CobaltStrike, and lateral movement. I have a curiosity that copy/pasting powershell commands is killing.

## Did you write this from the ground up?
The DCOM lateral movement took sometime to figure out, and I did not find it done in other projects/repos. However, the WMI lateral movement are mainly done by others. What I did was minor modifications and porting it to BOF.

## Note on quality
No. I am not a seasoned developer yet, so use with care. Before pushing these scripts to GIT, these scripts were tested on an Enterprise environment where network MDR is provided, and no alerts were trigged. However, it goes without saying that you should modify and test the scripts before you run them in your engagements. If you need assistant, please do not hesistate to contact me. Also, if you are interested in having aggressor scripts for these BOF, please lemme know!

## Can I/We reach you?
Yes, on[Twitter](https://twitter.com/Yas_o_h) or by [email](mailto:Y.Alhazmi@student.fontys.nl)

## Can I/We help you?
Yes, with a star, a retweet, or by inviting me to your Red Team after I graduate from university.

## Acknowledgement
Big thanks to [rsmudge](https://github.com/rsmudge) for his cintinous support and responsiveness to questions. The articles by [domchell](https://github.com/dmchell) served as a great introduction and helped in shaping my priorities.
