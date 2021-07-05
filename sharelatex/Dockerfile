FROM sharelatex/sharelatex

# Modified from https://github.com/rigon/docker-sharelatex-full/blob/master/Dockerfile

RUN set -x \
    && tlmgr init-usertree \
    # Select closest mirror automatically: http://tug.org/texlive/doc/install-tl.html
    #
    # or specify a TeX Live repository
    # && tlmgr option repository https://mirrors.ustc.edu.cn/CTAN/systems/texlive/tlnet/ \

    # Update & Install
    && tlmgr update --self \
    && tlmgr update --all \
    && tlmgr install scheme-full
