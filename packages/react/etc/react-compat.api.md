## API Report File for "@fluentui/react"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { IBaseProps } from '@fluentui/utilities';
import { IComponentAs } from '@fluentui/utilities';
import { IFocusZoneProps } from '@fluentui/react-focus';
import { IRectangle } from '@fluentui/utilities';
import { IRefObject } from '@fluentui/utilities';
import { IRenderFunction } from '@fluentui/utilities';
import { IStyle } from '@fluentui/style-utilities';
import { IStyleFunctionOrObject } from '@fluentui/utilities';
import { ITheme } from '@fluentui/style-utilities';
import { KeyCodes } from '@fluentui/utilities';
import { Point } from '@fluentui/utilities';
import * as React from 'react';
import { Target } from '@fluentui/react-hooks';

// @public (undocumented)
export class ActionButton extends React.Component<IButtonProps, {}> {
    // (undocumented)
    render(): JSX.Element;
}

// @public (undocumented)
export class BaseButton extends React.Component<IBaseButtonProps, IBaseButtonState> implements IButton {
    constructor(props: IBaseButtonProps);
    // (undocumented)
    componentDidMount(): void;
    // (undocumented)
    componentDidUpdate(prevProps: IBaseButtonProps, prevState: IBaseButtonState): void;
    // (undocumented)
    componentWillUnmount(): void;
    // (undocumented)
    static defaultProps: Partial<IBaseButtonProps>;
    // (undocumented)
    dismissMenu(): void;
    // (undocumented)
    focus(): void;
    // (undocumented)
    openMenu(shouldFocusOnContainer?: boolean, shouldFocusOnMount?: boolean): void;
    // (undocumented)
    render(): JSX.Element;
    }

// @public @deprecated
export class Button extends React.Component<IButtonProps, {}> {
    constructor(props: IButtonProps);
    // (undocumented)
    render(): JSX.Element;
}

// @public (undocumented)
export enum ButtonType {
    // (undocumented)
    command = 4,
    // (undocumented)
    compound = 3,
    // (undocumented)
    default = 6,
    // (undocumented)
    hero = 2,
    // (undocumented)
    icon = 5,
    // (undocumented)
    normal = 0,
    // (undocumented)
    primary = 1
}

// @public (undocumented)
export class CommandBarButton extends React.Component<IButtonProps, {}> {
    // (undocumented)
    render(): JSX.Element;
}

// @public (undocumented)
export const CommandButton: typeof ActionButton;

// @public (undocumented)
export class CompoundButton extends React.Component<IButtonProps, {}> {
    // (undocumented)
    render(): JSX.Element;
}

// @public (undocumented)
export class DefaultButton extends React.Component<IButtonProps, {}> {
    // (undocumented)
    render(): JSX.Element;
}

// @public (undocumented)
export enum ElementType {
    anchor = 1,
    button = 0
}

// @public (undocumented)
export const getSplitButtonClassNames: (styles: IButtonStyles, disabled: boolean, expanded: boolean, checked: boolean, primaryDisabled?: boolean | undefined) => ISplitButtonClassNames;

// @public (undocumented)
export interface IBaseButtonProps extends IButtonProps {
    // (undocumented)
    baseClassName?: string;
    // (undocumented)
    variantClassName?: string;
}

// @public (undocumented)
export interface IBaseButtonState {
    // (undocumented)
    menuHidden: boolean;
}

// @public (undocumented)
export interface IButton {
    dismissMenu: () => void;
    focus: () => void;
    openMenu: (shouldFocusOnContainer?: boolean, shouldFocusOnMount?: boolean) => void;
}

// @public (undocumented)
export interface IButtonClassNames {
    // (undocumented)
    description?: string;
    // (undocumented)
    flexContainer?: string;
    // (undocumented)
    icon?: string;
    // (undocumented)
    label?: string;
    // (undocumented)
    menuIcon?: string;
    // (undocumented)
    root?: string;
    // (undocumented)
    screenReaderText?: string;
    // (undocumented)
    textContainer?: string;
}

// @public (undocumented)
export interface IButtonProps extends React.AllHTMLAttributes<HTMLAnchorElement | HTMLButtonElement | HTMLDivElement | BaseButton | Button | HTMLSpanElement> {
    allowDisabledFocus?: boolean;
    ariaDescription?: string;
    ariaHidden?: boolean;
    ariaLabel?: string;
    // @deprecated (undocumented)
    buttonType?: ButtonType;
    checked?: boolean;
    className?: string;
    componentRef?: IRefObject<IButton>;
    data?: any;
    defaultRender?: any;
    // @deprecated
    description?: IStyle;
    disabled?: boolean;
    // @deprecated
    elementRef?: React.Ref<HTMLElement>;
    getClassNames?: (theme: ITheme, className: string, variantClassName: string, iconClassName: string | undefined, menuIconClassName: string | undefined, disabled: boolean, checked: boolean, expanded: boolean, hasMenu: boolean, isSplit: boolean | undefined, allowDisabledFocus: boolean) => IButtonClassNames;
    getSplitButtonClassNames?: (disabled: boolean, expanded: boolean, checked: boolean, allowDisabledFocus: boolean) => ISplitButtonClassNames;
    href?: string;
    // Warning: (ae-forgotten-export) The symbol "IIconProps" needs to be exported by the entry point index.d.ts
    iconProps?: IIconProps;
    // Warning: (ae-forgotten-export) The symbol "IKeytipProps" needs to be exported by the entry point index.d.ts
    keytipProps?: IKeytipProps;
    menuAs?: IComponentAs<IContextualMenuProps>;
    menuIconProps?: IIconProps;
    // Warning: (ae-forgotten-export) The symbol "IContextualMenuProps" needs to be exported by the entry point index.d.ts
    menuProps?: IContextualMenuProps;
    menuTriggerKeyCode?: KeyCodes | null;
    onAfterMenuDismiss?: () => void;
    onMenuClick?: (ev?: React.MouseEvent<HTMLElement> | React.KeyboardEvent<HTMLElement>, button?: IButtonProps) => void;
    onRenderAriaDescription?: IRenderFunction<IButtonProps>;
    onRenderChildren?: IRenderFunction<IButtonProps>;
    onRenderDescription?: IRenderFunction<IButtonProps>;
    onRenderIcon?: IRenderFunction<IButtonProps>;
    // @deprecated (undocumented)
    onRenderMenu?: IRenderFunction<IContextualMenuProps>;
    onRenderMenuIcon?: IRenderFunction<IButtonProps>;
    onRenderText?: IRenderFunction<IButtonProps>;
    persistMenu?: boolean;
    primary?: boolean;
    primaryActionButtonProps?: IButtonProps;
    primaryDisabled?: boolean;
    // @deprecated
    renderPersistedMenuHiddenOnMount?: boolean;
    // @deprecated (undocumented)
    rootProps?: React.ButtonHTMLAttributes<HTMLButtonElement> | React.AnchorHTMLAttributes<HTMLAnchorElement>;
    secondaryText?: string;
    split?: boolean;
    splitButtonAriaLabel?: string;
    splitButtonMenuProps?: IButtonProps;
    styles?: IButtonStyles;
    text?: string;
    theme?: ITheme;
    toggle?: boolean;
    // @deprecated (undocumented)
    toggled?: boolean;
    uniqueId?: string | number;
}

// @public (undocumented)
export interface IButtonStyles {
    description?: IStyle;
    descriptionChecked?: IStyle;
    descriptionDisabled?: IStyle;
    descriptionHovered?: IStyle;
    descriptionPressed?: IStyle;
    flexContainer?: IStyle;
    icon?: IStyle;
    iconChecked?: IStyle;
    iconDisabled?: IStyle;
    iconExpanded?: IStyle;
    iconExpandedHovered?: IStyle;
    iconHovered?: IStyle;
    iconPressed?: IStyle;
    label?: IStyle;
    labelChecked?: IStyle;
    labelDisabled?: IStyle;
    labelHovered?: IStyle;
    menuIcon?: IStyle;
    menuIconChecked?: IStyle;
    menuIconDisabled?: IStyle;
    menuIconExpanded?: IStyle;
    menuIconExpandedHovered?: IStyle;
    menuIconHovered?: IStyle;
    menuIconPressed?: IStyle;
    root?: IStyle;
    rootChecked?: IStyle;
    rootCheckedDisabled?: IStyle;
    rootCheckedHovered?: IStyle;
    rootCheckedPressed?: IStyle;
    rootDisabled?: IStyle;
    rootExpanded?: IStyle;
    rootExpandedHovered?: IStyle;
    rootFocused?: IStyle;
    rootHasMenu?: IStyle;
    rootHovered?: IStyle;
    rootPressed?: IStyle;
    screenReaderText?: IStyle;
    secondaryText?: IStyle;
    splitButtonContainer?: IStyle;
    splitButtonContainerChecked?: IStyle;
    splitButtonContainerCheckedHovered?: IStyle;
    splitButtonContainerDisabled?: IStyle;
    splitButtonContainerFocused?: IStyle;
    splitButtonContainerHovered?: IStyle;
    splitButtonDivider?: IStyle;
    splitButtonDividerDisabled?: IStyle;
    splitButtonFlexContainer?: IStyle;
    splitButtonMenuButton?: IStyle;
    splitButtonMenuButtonChecked?: IStyle;
    splitButtonMenuButtonDisabled?: IStyle;
    splitButtonMenuButtonExpanded?: IStyle;
    splitButtonMenuIcon?: IStyle;
    splitButtonMenuIconDisabled?: IStyle;
    textContainer?: IStyle;
}

// @public (undocumented)
export class IconButton extends React.Component<IButtonProps, {}> {
    // (undocumented)
    render(): JSX.Element;
}

// @public (undocumented)
export interface ISplitButtonClassNames {
    // (undocumented)
    divider?: string;
    // (undocumented)
    flexContainer?: string;
    // (undocumented)
    icon?: string;
    // (undocumented)
    root?: string;
    // (undocumented)
    splitButtonContainer?: string;
}

// @public (undocumented)
export class MessageBarButton extends React.Component<IButtonProps, {}> {
    // (undocumented)
    render(): JSX.Element;
}

// @public (undocumented)
export class PrimaryButton extends React.Component<IButtonProps, {}> {
    // (undocumented)
    render(): JSX.Element;
}


// (No @packageDocumentation comment for this package)

```