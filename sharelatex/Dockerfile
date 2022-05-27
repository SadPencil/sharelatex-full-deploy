FROM sharelatex/sharelatex:3.0.1

# Modified from https://github.com/rigon/docker-sharelatex-full/blob/master/Dockerfile

RUN set -x \
    && tlmgr init-usertree \
    && tlmgr option repository https://ftp.math.utah.edu/pub/tex/historic/systems/texlive/2021/tlnet-final \
    # && tlmgr option repository https://mirrors.tuna.tsinghua.edu.cn/tex-historic-archive/systems/texlive/2021/tlnet-final/ \
    # Update
    && tlmgr update --self \
    && tlmgr update --all \
    && tlmgr install scheme-full
