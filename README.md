## Parsnp Analysis on Campylobacter jejuni isolates
- **CPU Architecture**: x86_64 (2-core)
- **Machine**: HP Spectre
- **Operating System**: Ubuntu 22.04 LTS
- **Parsnp Version**: v1.5.6
- **OS Compatibility**: Linux, macOS - Windows users are advised to use WSL or a virtual machine for compatibility.
- **Input**: Group D1's Skesa + Trimmomatic Assemblies (.fasta or .fna files), please download these to your repo prior to proceeding
- **Reference Genome**: D0287766_S01_L001-SKESA_contigs.fasta (chosen due to QUAST quality assessment)
## Main commands needed to run Parsnp are seen here. Please replace input and output directories as needed.
```bash
parsnp -r /home/username/group4/input-sequences-final/D0287766_S01_L001-SKESA_contigs.fasta \
       -d /home/username/group4/input-sequences-final \
       -o /home/username/group4/output_dir_D0287766_reference > D0287766_log.txt 2>&1

figtree ~/group4/output_dir_D0287766_reference/parsnp.tree
```
