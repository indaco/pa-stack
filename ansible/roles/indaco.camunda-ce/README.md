# indaco.camunda-ce

It takes care of the entire setup for the bpm stack.

- Create needed folders
- Create needed configuration files
- Pull docker images from docher hub
- Run the docker compose stack

## Example Playbook

    - hosts: all
      roles:
         - role: indaco.camunda-ce

## License

MIT
