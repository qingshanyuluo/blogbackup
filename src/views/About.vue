<template>
  <div class="page-about">
    <div class="list">
      <div class="item">
        <h3>是一只可爱的嘀嘀嘀</h3>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  setup() {
    return {

    };
  },
};
</script>
<style lang="scss" scoped>
  .pc-mode {
    .page-about {
      .projects {
        .project {
          a { margin-left: -26px;}
        }
      }
    }
  }
  .page-about {
    .list {
      .item {
        &-name { position: relative; height: 32px;
          h4 { font-weight: bold; font-size: $sizeLarge; color: $mainStrong; line-height: 1.5;}
        }
      }
      .item + .item { padding-top: 16px;}
    }
    .projects { margin-top: 24px; margin-bottom: 16px; list-style: none;
      .project {
        a { position: relative; cursor: auto;
          h4 { font-size: $sizeMedium; color: $mainStrong; line-height: 1.5; white-space: nowrap; text-overflow: ellipsis; overflow: hidden; transition: all $animateTime; cursor: pointer;
            &:hover,&:active { color: #1abc9c;}
          }
          i { color: $main; transition: color $animateTime; cursor: pointer; margin-right: 10px;
            &:hover,&:active { color: $mainStrong;}
          }
          img { cursor: pointer; margin-left: 8px;}
        }
        p { color: $main; font-size: $sizeNormal; line-height: 1.5; margin-top: 8px;}
        &.private { cursor: not-allowed; pointer-events: none; opacity: 0.5;}
      }
      .project + .project { margin-top: 24px;}
    }
  }
</style>
