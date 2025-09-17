FROM docker.io/searxng/searxng:latest

# settings.yml 복사
COPY settings.yml /etc/searxng/settings.yml

# 캐시 디렉토리 생성 및 권한 설정
RUN mkdir -p /var/cache/searxng && \
    chown -R searxng:searxng /var/cache/searxng

# 환경 변수 기본값 설정 (필요시)
ENV SEARXNG_BASE_URL=https://localhost/