FROM quay.io/operator-framework/ansible-operator:v0.19.2

USER root
RUN dnf install -y git python3 && pip3 install jmespath

USER ${USER_UID}

COPY requirements.yml ${HOME}/requirements.yml
RUN ansible-galaxy collection install -r ${HOME}/requirements.yml \
 && chmod -R ug+rwx ${HOME}/.ansible

COPY watches.yaml ${HOME}/watches.yaml
COPY roles/ ${HOME}/roles/


