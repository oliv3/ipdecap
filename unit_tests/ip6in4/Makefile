check: clean process_pcap compare_md5

clean:
	@echo "*** Cleaning decapsulated pcap files..."
	-rm -vf *.cap.output

process_pcap: 
	@echo "*** Processing gre_version0.cap..."
	../../ipdecap -i ip6in4.cap -o ip6in4.cap.output

compare_md5:
	@echo "*** Comparing checksums..."
	md5sum -c ip6in4.md5
	

.PHONY = check
