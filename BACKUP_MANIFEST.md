# Backup manifest

This is a clean source snapshot of the thesis LLM setup component; the larger thesis repository history is omitted because it contains credential-bearing configuration in a separate embedded project. The original Git repository and files remain unchanged.

Sensitive `api_key`, `master_key`, `default_api_key`, and host fields in the copied LiteLLM/vLLM configuration are blanked. The source also has local `.env` files outside this component; they are not included.

Excluded local state:

- `test_results/`, runtime logs, PIDs, outputs, and Slurm job output.
- `.orig` backups, local environments, caches, model files, and generated artifacts.

Rotate any copied key fields if their original values were valid credentials.
