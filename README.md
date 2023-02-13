# blast


# conda env 
conda activate V05_236_BLAST

# make database
makeblastdb -in MPXVdb -dbtype nucl


# Run local data aganist the database  
blastn -num_threads 60 -outfmt 6 -db local_db -query query.fasta -out results.blastn

