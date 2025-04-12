# Action-Setup-SSH

A GitHub Action to configure SSH keys and host fingerprints.

> Note: This is not a generic SSH utility action. It's built to support my own workflows and nothing more.

## Usage

```yml
- name: Setup Godot
  uses: SolarLabyrinth/Action-Setup-SSH@v1
  with:
    name: id_ed25519
    public_key: ${{ secrets.DEPLOY_PUBLIC_KEY }}
    private_key: ${{ secrets.DEPLOY_PRIVATE_KEY }}
    host: ${{ secrets.DEPLOY_HOST }}
    port: ${{ secrets.DEPLOY_PORT }}
```
