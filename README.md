# bu-usb_backup_tool SolusOS edition

1. Description:

 BU is a program that makes keeping all of your user data safely backed up on
 a dedicated External USB drive easy. It is a leaner meaner version of the XBT
 backup script that came before it. 

 BU will update files that have changed, remove files that have been
 deleted and add any new files that have been created since the last backup.
 The initial backup can take a lot of time if you have a lot of data stored
 in your system's /home directory. BU creates a directory with the host name
 of the machine it's backing up from inside BU_Backups. This allows users to
 share one BU_Drive with multiple machines.


2. Installation:

 Unzip the "bu" bash script from the zip archive and move it to either
 /usr/local/bin or ~/bin. You can either do this from a command line or simply
 drag the file out of Archive Manager to wherever you'd like it to go.


3. License.

 BU is free softare. You can redistribute it and/or modify it under the
 terms of the GNU General Public License Version 2.0. as published by
 the Free Software Foundation. A copy of the GNU GPL 2.0 is provided with the
 software.

4. Contents of Help Page:

 BU - USB Backup Tool (Version 1.0) -- Help
 (v. 1.0)

 Press "q" to exit this Help page.

 Commands:

 bu = Fully backs up host's /etc and /home directories to BU_Drive.
 bu --help = Prints this help information.
 bu --restore = Accesses BU Restore function.

 Description:

 BU is a program that makes keeping all of your user data safely backed up on
 a dedicated External USB drive easy.

 BU will update files that have changed, remove files that have been
 deleted and add any new files that have been created since the last backup.
 The initial backup can take a lot of time if you have a lot of data stored
 in your system's /home directory. BU creates a directory with the host name
 of the machine it's backing up from inside BU_Backups. This allows users to
 share one BU_Drive with multiple machines.

 The directory structure and all files are stored openly to allow users easy
 access if they only need to retrieve a few files or directories using a file
 manager.

 The BU Restore function is an interactive tool that let's users restore their
 /home directories to a backup up state. This function will only work when
 restoring to a machine with the exact same hostname as the one the backs were
 made from. It is intended for emergency use, as when significant number of
 directories and files are accidentally removed from /home.

 BU_Drive Setup

 You need to prepare a BU Drive with a tool like Gparted or Disks.
 This can be any USB storage device. The dedicated USB drive MUST contain a
 partition formatted with a Linux native file system such as Ext4 or XFS. The
 partition MUST be labeled "BU_Drive" so BU can find it and use it for backups.
 The partition needs to have enough free capacity to store all data in /home on
 all of the machines you want to use the drive for. Note: You will get many
 errors if you attempt to use BU to backup to a partition that is formatted with
 non-native file systems like FAT32 or NTFS. 

 Disclaimer:

 THIS SOFTWARE IS PROVIDED BY EZEELINUX “AS IS” AND ANY EXPRESS OR IMPLIED
 WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
 MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
 EVENT SHALL EZEELINUX BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.

