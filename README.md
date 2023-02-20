regional_import - Main procedure.
It reads Images from disks, import to NetBackup. duplication into tapes, mark disk copy to delete.
Usage:
nohup ./regional_import > regional_import.out 2>&1 &

regional_disk_images_check - Check disk Images for bugs.
Usage:
./regional_disk_images_check > regional_disk_images_check.out 2>&1

dirname: missing operand
Try 'dirname --help' for more information.

That message occurs when images on some disk are absent. 

regional_emm_status - It writes into file regional_emm_status.txt report for images in NetBackup base: 
State, Disk copy exists, File Name on disk, файлов на дисках, Tape Name for Image Copy, Create Image Date, Expire Image Date.
Usage:
./regional_emm_status > regional_emm_status.txt 2>&1

regional_watchdog - Autoexecution procedure by cron.
Sample:
0 0,12 * * * /root/regional/regional_watchdog >> /root/regional/regional_watchdog.out 2>&1

image_info - Get info for some Image.

regional_disk_images_delete - It delete Images from disk, for which tape copy is done.
Usage:
./regional_disk_images_delete > regional_disk_images_delete.out 2>&1

regional_disks_image_dubles - It search Image Dubbles on disks.

regional_disks_status - It count and displays Disk Image State.

regional_emm_clear_disks_copies - It mark Image disk copy in NetBackup Base to delete, for which tape copy is done.
Usage:
./regional_emm_clear_disks_copies > regional_emm_clear_disks_copies.out 2>&1

regional_img_sort - It sorts Images on disks by write time into disk.

